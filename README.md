## Solomining proxy for equihash coins like Zclassic, Zcash, and ZeroClassic.
## (READY FOR TESTING)

Made by the Zclassic community, configuration and documentation is ~~[here](https://zdeveloper.org/equihash-solomining)~~

Updated/tweaked by Potato from the ZeroClassic community

![picture alt](http://i.imgur.com/xB9XdVF.png)

Requirements
------------
* node
* coin daemon

Install
-------------

```bash
sudo apt-get install build-essential libsodium-dev npm
sudo npm install n -g
sudo n stable
git clone https://github.com/zzzpotato/solo-nomp
cd solo-nomp
npm update
npm install
```

Configure
-------------
Rename config_example.json and change it to your setup. Official documentation is here: ~~[https://zdeveloper.org/equihash-solomining](https://zdeveloper.org/equihash-solomining)~~

Start
------------
```bash
npm start
```

PM2 Start
------------
```bash
pm2 start init.js --name solo
```

Update
-------------
Get rid of the node_modules folder then 
```bash
npm install
git pull
```

Differences between this and S-NOMP
------------
* This is meant for solo mining
* There is no share system; Every "share" is the block solution
* No payment processor, you will need to shield rewards to spend them yourself

Upcoming Feautures
-------------
* More API
* Web interface changes

Support
-------------
* ~~https://gitter.im/equihash-solomining~~
* Potato#9721 on Discord

License
-------
Released under the GNU General Public License v2
http://www.gnu.org/licenses/gpl-2.0.html

_Forked from [z-classic/node-stratum-pool](https://github.com/z-classic/node-stratum-pool) which is licensed under GNU GPL v2_
