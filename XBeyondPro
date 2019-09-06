#!/bin/sh
#CDIR=$(cd "`dirname \"$0\"`"; pwd)
#CDIR="/Users/admin/Applications/Beyond Compare.app"
#sudo mkdir -p /usr/local/bin/
#sudo ln -sf "$CDIR/Contents/MacOS/bcomp" /usr/local/bin/

rm -rf ~/Library/Application\ Support/Beyond\ Compare
mkdir -p ~/Library/Application\ Support/Beyond\ Compare
echo 1 > ~/Library/Application\ Support/Beyond\ Compare/IsPro
touch ~/Library/Application\ Support/Beyond\ Compare/registry.dat
chmod 000 ~/Library/Application\ Support/Beyond\ Compare/registry.dat

cat << EOF | tee ~/Library/Application\ Support/Beyond\ Compare/BCCommands.xml > /dev/null
<?xml version="1.0" encoding="UTF-8"?>
<!-- Produced by Beyond Compare 4 from Scooter Software -->
<BCCommands Version="1" MinVersion="1">
	<TDirCompareCommands>
		<Items>
			<DeleteAction Value=";;True"/>
			<MoveAction Value=";;True"/>
			<MirrorLeftAction Value=";;True"/>
			<MirrorRightAction Value=";;True"/>
			<NameFilterEditAction Value=";;False"/>
		</Items>
	</TDirCompareCommands>
</BCCommands>
EOF

cat << EOF | tee ~/Library/Application\ Support/Beyond\ Compare/BCPreferences.xml > /dev/null
<?xml version="1.0" encoding="UTF-8"?>
<!-- Produced by Beyond Compare 4 from Scooter Software -->
<BCPreferences Version="1" MinVersion="1">
	<TBcPrefs>
		<OpConfirmCopy Value="False"/>
	</TBcPrefs>
</BCPreferences>
EOF
