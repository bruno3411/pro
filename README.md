
<html lang="lv">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Reģistrēt jaunu personu SAIS</title>
<style>
/* Layout: pixel replica of the Oracle Forms screen JUBU0104 (1168x634); every element is absolutely placed at coordinates measured from the reference screenshot. */
:root{
  --stage:#cfd3d3;
  --canvas:#f4f4f4;
  --group:#e0e0e0;
  --group-edge:#a8c3bf;
  --title:#344c4c;
  --title-strip:#8fb5b4;
  --fld-grey:#eaeaea;
  --fld-cyan:#befeff;
  --fld-white:#fbffff;
  --bd-dark:#84b2ab;
  --bd-light:#d3e0df;
  --btn:#bfbfbf;
  --ink:#141414;
  --txt:#1e1e1e;
  --ok:#0b5d24;
  color-scheme:light;
}
body{margin:0;background:var(--stage);color:var(--ink);font-family:Arial,"Liberation Sans",Helvetica,sans-serif;padding-inline:16px;padding-block:16px}
.stage{overflow-x:auto;max-width:100%}
.win{position:relative;width:1168px;height:634px;background:var(--canvas);margin:0 auto;overflow:hidden;font-size:13px}
.win[hidden]{display:none}
.tbtop{position:absolute;left:0;top:0;width:1168px;height:3px;background:var(--title-strip)}
.tb{position:absolute;left:0;top:3px;width:1168px;height:17px;background:var(--title)}
.tb:after{content:"";position:absolute;left:0;top:17px;width:1168px;height:1px;background:#c9cfcd}
.tt{position:absolute;top:5px;font-size:11.75px;line-height:14px;color:#f2f2f2;white-space:nowrap}
.ico{position:absolute;left:2px;top:5px;width:11px;height:12px;background:#3f86d6;border-radius:2px 4px 2px 2px}
.ico:after{content:"";position:absolute;left:2px;top:4px;width:5px;height:4px;border:1px solid #fff;border-radius:1px;box-sizing:border-box}
.wr{position:absolute;left:1148px;top:9px;width:8px;height:7px;border:1px solid #dfe6e6;box-sizing:border-box}
.wr:after{content:"";position:absolute;left:-3px;top:2px;width:7px;height:6px;border:1px solid #dfe6e6;background:var(--title);box-sizing:border-box}
.wx{position:absolute;left:1159px;top:6px;width:8px;height:12px;font:normal 14px/12px Arial,sans-serif;color:#e6eaea}
.wx:after{content:"\2715";font-size:10px}
.bb{position:absolute;left:0;top:632px;width:1168px;height:2px;background:linear-gradient(#a2b8b6 50%,#697f7e 50%)}
.grp{position:absolute;box-sizing:border-box;background:var(--group);border:1px solid var(--group-edge);border-radius:4px;box-shadow:0 0 0 1px #e6f1ef}
.gt{position:absolute;font-weight:700;font-size:14.4px;line-height:17px;white-space:nowrap;color:#000}
.lb{position:absolute;font-size:13px;line-height:15px;white-space:nowrap;color:var(--txt)}
.f{position:absolute;box-sizing:border-box;margin:0;padding:0 1px 0 1px;font:13px Arial,"Liberation Sans",sans-serif;color:#000;border-style:solid;border-width:2px 1px 1px 2px;border-color:var(--bd-dark) var(--bd-light) var(--bd-light) var(--bd-dark);border-radius:0;outline:0}
.f.gr{background:var(--fld-grey)}
.f.cy{background:var(--fld-cyan)}
.f.wh{background:var(--fld-white)}
.f:focus{box-shadow:inset 0 0 0 1px #1f5fbf}
.f.bad{background:#ffbcbc}
.f::placeholder{color:#7a7a7a}
.f:disabled{color:#000;opacity:1}
.sel{position:absolute;background:#0000ff;color:#fff;font-size:13px;line-height:17px;padding:0 1px;pointer-events:none;z-index:2}
.btn{position:absolute;box-sizing:border-box;margin:0;padding:0;font:700 13px Arial,"Liberation Sans",sans-serif;color:#111;background:var(--btn);border:1px solid;border-color:#f0f0f0 #9ca2a2 #9ca2a2 #f0f0f0;border-radius:0;cursor:pointer;box-shadow:inset 1px 1px 0 #cdcdcd}
.btn:hover{background:#c8c8c8}
.btn:active{background:#b0b0b0;border-color:#9ca2a2 #f0f0f0 #f0f0f0 #9ca2a2}
.btn:focus-visible{outline:1px dotted #000;outline-offset:-5px}
.btn:disabled{color:#9d9d9d;text-shadow:1px 1px 0 #eee;cursor:default;background:var(--btn)}
.sb{position:absolute;box-sizing:border-box;background:#cdcdcd;border:1px solid #bdc7c6;border-radius:3px}
.sb i{position:absolute;left:0;right:0;height:13px;background:#d9dada;border:1px solid #aab4b3;border-radius:3px;box-sizing:border-box}
.sb .up{top:0}.sb .dn{bottom:0}
.sb i:after{content:"";position:absolute;left:50%;top:4px;margin-left:-3px;border:3px solid transparent}
.sb .up:after{border-bottom:4px solid #555;border-top:0}
.sb .dn:after{border-top:4px solid #555;border-bottom:0;top:5px}
.sb b{position:absolute;left:3px;right:3px;top:50%;height:12px;margin-top:-6px;background:radial-gradient(#fff 1px,transparent 1.4px) 0 0/4px 4px}
.dlg{position:absolute;left:410px;top:220px;width:300px;height:124px;background:var(--group);border:1px solid #6d8a87;box-shadow:3px 3px 0 rgba(0,0,0,.25);z-index:5}
.dlg[hidden]{display:none}
.dh{height:17px;background:var(--title);color:#fff;font-size:11.75px;line-height:17px;padding-left:8px}
.dm{padding:8px 10px;font-size:13px;line-height:16px;height:44px}
.note{max-width:1168px;margin:10px auto 0;font-size:12px;color:#333}
</style>
</head>
<body>
<div class="stage">
<form class="win" id="s1" novalidate><div class="tbtop"></div><div class="tb"></div><i class="ico"></i><div class="tt" style="left:14px">SED identificējamo personu dati</div><div class="tt" style="left:676px">Starptautisko pakalpojumu nodaļa&nbsp;&nbsp;&nbsp;JUBU0104</div><i class="wr"></i><i class="wx"></i><div class="grp" style="left:7px;top:26px;width:960px;height:73px"></div>
<div class="gt" style="left:39px;top:28.7px">Informācija par SED</div>
<div class="lb " style="left:-163px;top:52.9px;width:300px;text-align:right">Lietas Nr. (RINA)</div>
<div class="lb " style="left:-163px;top:73.9px;width:300px;text-align:right">Izdevējvalsts</div>
<div class="lb " style="left:145px;top:52.9px;width:300px;text-align:right">Dokumenta tips</div>
<div class="lb " style="left:144px;top:74.30000000000001px;width:300px;text-align:right">Izdevējorganizācija</div>
<input id="s1-lieta" class="f gr" style="left:141px;top:49px;width:186px;height:22px" value="3570" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-izv" class="f gr" style="left:141px;top:71px;width:186px;height:22px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-dok" class="f gr" style="left:446px;top:49px;width:306px;height:22px" value="H001 Paziņojums/ informācijas pieprasījums" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-izo" class="f gr" style="left:446px;top:71px;width:306px;height:22px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<button type="button" id="s1-json" class="btn " style="left:768px;top:50px;width:165px;height:31px">SED saturs (JSON)</button>
<div class="grp" style="left:7px;top:106px;width:960px;height:189px"></div>
<div class="gt" style="left:39px;top:107.7px">Identificējamo personu dati</div>
<div class="lb " style="left:690px;top:126.9px;width:300px;text-align:left">Dzimšanas</div>
<div class="lb " style="left:766px;top:126.9px;width:300px;text-align:left">Miršanas</div>
<div class="lb " style="left:842px;top:126.9px;width:300px;text-align:left">SAIS personas</div>
<div class="lb " style="left:26px;top:144.9px;width:300px;text-align:left">Identifikācijas kods</div>
<div class="lb " style="left:143px;top:144.9px;width:300px;text-align:left">Valsts</div>
<div class="lb " style="left:269px;top:145.9px;width:300px;text-align:left">Uzvārds (transliterācijā)</div>
<div class="lb " style="left:462px;top:145.9px;width:300px;text-align:left">Vārds (i) (transliterācijā)</div>
<div class="lb " style="left:649px;top:144.9px;width:300px;text-align:left">Dzim</div>
<div class="lb " style="left:689px;top:145.9px;width:300px;text-align:left">datums</div>
<div class="lb " style="left:766px;top:145.9px;width:300px;text-align:left">datums</div>
<div class="lb " style="left:842px;top:145.9px;width:300px;text-align:left">kods</div>
<input id="s1-id0" class="f cy" style="left:25px;top:160px;width:109px;height:21px" value="1234-5678" autocomplete="off" spellcheck="false">
<input id="s1-valsts0" class="f cy" style="left:141px;top:160px;width:126px;height:21px" value="BULGĀRIJA" autocomplete="off" spellcheck="false">
<input id="s1-uzv0" class="f cy" style="padding-left:0px;left:270px;top:160px;width:186px;height:21px" value="BERZINS" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-vards0" class="f cy" style="padding-left:0px;left:460px;top:160px;width:186px;height:21px" value="JANIS" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-dzim0" class="f cy" style="left:649px;top:160px;width:37px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-dzd0" class="f cy" style="padding-left:3px;left:689px;top:160px;width:73px;height:21px" value="11.11.1911." data-p="3" autocomplete="off" spellcheck="false">
<input id="s1-mird0" class="f cy" style="left:765px;top:160px;width:73px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-sais0" class="f cy" style="left:841px;top:160px;width:85px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-id1" class="f gr" style="left:25px;top:182px;width:109px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-valsts1" class="f gr" style="left:141px;top:182px;width:126px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-uzv1" class="f gr" style="padding-left:0px;left:270px;top:182px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-vards1" class="f gr" style="padding-left:0px;left:460px;top:182px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-dzim1" class="f gr" style="left:649px;top:182px;width:37px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-dzd1" class="f gr" style="padding-left:3px;left:689px;top:182px;width:73px;height:21px" value="" data-p="3" autocomplete="off" spellcheck="false">
<input id="s1-mird1" class="f gr" style="left:765px;top:182px;width:73px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-sais1" class="f gr" style="left:841px;top:182px;width:85px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-id2" class="f gr" style="left:25px;top:203px;width:109px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-valsts2" class="f gr" style="left:141px;top:203px;width:126px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-uzv2" class="f gr" style="padding-left:0px;left:270px;top:203px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-vards2" class="f gr" style="padding-left:0px;left:460px;top:203px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-dzim2" class="f gr" style="left:649px;top:203px;width:37px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-dzd2" class="f gr" style="padding-left:3px;left:689px;top:203px;width:73px;height:21px" value="" data-p="3" autocomplete="off" spellcheck="false">
<input id="s1-mird2" class="f gr" style="left:765px;top:203px;width:73px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-sais2" class="f gr" style="left:841px;top:203px;width:85px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-id3" class="f gr" style="left:25px;top:224px;width:109px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-valsts3" class="f gr" style="left:141px;top:224px;width:126px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-uzv3" class="f gr" style="padding-left:0px;left:270px;top:224px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-vards3" class="f gr" style="padding-left:0px;left:460px;top:224px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-dzim3" class="f gr" style="left:649px;top:224px;width:37px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-dzd3" class="f gr" style="padding-left:3px;left:689px;top:224px;width:73px;height:21px" value="" data-p="3" autocomplete="off" spellcheck="false">
<input id="s1-mird3" class="f gr" style="left:765px;top:224px;width:73px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-sais3" class="f gr" style="left:841px;top:224px;width:85px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-id4" class="f gr" style="left:25px;top:246px;width:109px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-valsts4" class="f gr" style="left:141px;top:246px;width:126px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-uzv4" class="f gr" style="padding-left:0px;left:270px;top:246px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-vards4" class="f gr" style="padding-left:0px;left:460px;top:246px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-dzim4" class="f gr" style="left:649px;top:246px;width:37px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-dzd4" class="f gr" style="padding-left:3px;left:689px;top:246px;width:73px;height:21px" value="" data-p="3" autocomplete="off" spellcheck="false">
<input id="s1-mird4" class="f gr" style="left:765px;top:246px;width:73px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-sais4" class="f gr" style="left:841px;top:246px;width:85px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-id5" class="f gr" style="left:25px;top:267px;width:109px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-valsts5" class="f gr" style="left:141px;top:267px;width:126px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-uzv5" class="f gr" style="padding-left:0px;left:270px;top:267px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-vards5" class="f gr" style="padding-left:0px;left:460px;top:267px;width:186px;height:21px" value="" data-p="0" autocomplete="off" spellcheck="false">
<input id="s1-dzim5" class="f gr" style="left:649px;top:267px;width:37px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-dzd5" class="f gr" style="padding-left:3px;left:689px;top:267px;width:73px;height:21px" value="" data-p="3" autocomplete="off" spellcheck="false">
<input id="s1-mird5" class="f gr" style="left:765px;top:267px;width:73px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-sais5" class="f gr" style="left:841px;top:267px;width:85px;height:21px" value="" autocomplete="off" spellcheck="false">
<div class="sb" style="left:929px;top:160px;width:16px;height:129px"><i class="up"></i><i class="dn"></i><b></b></div>
<div class="grp" style="left:7px;top:302px;width:590px;height:153px"></div>
<div class="gt" style="left:39px;top:304.7px">Visi identifikācijas kodi</div>
<div class="lb " style="left:26px;top:325.29999999999995px;width:300px;text-align:left">Identifikācijas kods</div>
<div class="lb " style="left:154px;top:325.29999999999995px;width:300px;text-align:left">Valsts</div>
<div class="lb " style="left:255px;top:325.29999999999995px;width:300px;text-align:left">Organizācija</div>
<input id="s1-k0a" class="f cy" style="left:25px;top:340px;width:127px;height:21px" value="1234-5678" autocomplete="off" spellcheck="false">
<input id="s1-k0b" class="f cy" style="left:153px;top:340px;width:100px;height:21px" value="BULGĀRIJA" autocomplete="off" spellcheck="false">
<input id="s1-k0c" class="f cy" style="left:254px;top:340px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k1a" class="f gr" style="left:25px;top:362px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k1b" class="f gr" style="left:153px;top:362px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k1c" class="f gr" style="left:254px;top:362px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k2a" class="f gr" style="left:25px;top:383px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k2b" class="f gr" style="left:153px;top:383px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k2c" class="f gr" style="left:254px;top:383px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k3a" class="f gr" style="left:25px;top:405px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k3b" class="f gr" style="left:153px;top:405px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k3c" class="f gr" style="left:254px;top:405px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k4a" class="f gr" style="left:25px;top:426px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k4b" class="f gr" style="left:153px;top:426px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s1-k4c" class="f gr" style="left:254px;top:426px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<div class="sb" style="left:562px;top:340px;width:14px;height:108px"><i class="up"></i><i class="dn"></i><b></b></div>
<button type="button" id="s1-mekl" class="btn " style="left:727px;top:303px;width:163px;height:31px">Meklēt personu SAIS</button>
<button type="button" id="s1-regnew" class="btn newbtn" style="left:706px;top:338px;width:205px;height:31px">Reģistrēt jaunu personu SAIS</button>
<div class="grp" style="left:605px;top:378px;width:338px;height:119px"></div>
<div class="gt" style="left:637px;top:380.7px">Adrese</div>
<div class="lb " style="left:409px;top:404.9px;width:300px;text-align:right">Valsts</div>
<div class="lb " style="left:409px;top:425.9px;width:300px;text-align:right">Pilsēta/rajons</div>
<div class="lb " style="left:409px;top:447.9px;width:300px;text-align:right">Iela/māja</div>
<div class="lb " style="left:409px;top:467.9px;width:300px;text-align:right">Pasta indekss</div>
<input id="s1-a0" class="f gr" style="left:710px;top:401px;width:211px;height:21px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-a1" class="f gr" style="left:710px;top:422px;width:211px;height:21px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-a2" class="f gr" style="left:710px;top:444px;width:211px;height:21px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-a3" class="f gr" style="left:710px;top:465px;width:187px;height:21px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<div class="grp" style="left:7px;top:458px;width:564px;height:92px"></div>
<div class="gt" style="left:39px;top:460.7px">Piesaistāmā persona</div>
<div class="lb " style="left:-170px;top:483.9px;width:300px;text-align:right">Personas kods</div>
<div class="lb " style="left:-172px;top:505.9px;width:300px;text-align:right">Vārds (i)</div>
<div class="lb " style="left:-170px;top:526.9px;width:300px;text-align:right">Uzvārds</div>
<input id="s1-pkods" class="f wh" style="left:132px;top:480px;width:126px;height:22px" value="" autocomplete="off" spellcheck="false">
<input id="s1-pvards" class="f gr" style="left:132px;top:502px;width:187px;height:21px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s1-puzv" class="f gr" style="left:132px;top:523px;width:187px;height:21px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<button type="button" id="s1-pies" class="btn " style="left:334px;top:512px;width:206px;height:28px" disabled>Piesaistīt SAIS personu</button><div class="bb"></div></form>
<form class="win" id="s2" novalidate hidden><div class="tbtop"></div><div class="tb"></div><i class="ico"></i><div class="tt" style="left:14px">Reģistrēt jaunu personu SAIS</div><div class="tt" style="left:676px">Starptautisko pakalpojumu nodaļa&nbsp;&nbsp;&nbsp;JUBU0105</div><i class="wr"></i><i class="wx"></i><div class="grp" style="left:7px;top:26px;width:960px;height:73px"></div>
<div class="gt" style="left:39px;top:28.7px">Informācija par SED</div>
<div class="lb " style="left:-163px;top:52.9px;width:300px;text-align:right">Lietas Nr. (RINA)</div>
<div class="lb " style="left:-163px;top:73.9px;width:300px;text-align:right">Izdevējvalsts</div>
<div class="lb " style="left:145px;top:52.9px;width:300px;text-align:right">Dokumenta tips</div>
<div class="lb " style="left:144px;top:74.30000000000001px;width:300px;text-align:right">Izdevējorganizācija</div>
<input id="s2-lieta" class="f gr" style="left:141px;top:49px;width:186px;height:22px" value="3570" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s2-izv" class="f gr" style="left:141px;top:71px;width:186px;height:22px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s2-dok" class="f gr" style="left:446px;top:49px;width:306px;height:22px" value="H001 Paziņojums/ informācijas pieprasījums" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<input id="s2-izo" class="f gr" style="left:446px;top:71px;width:306px;height:22px" value="" readonly tabindex="-1" autocomplete="off" spellcheck="false">
<div class="grp" style="left:7px;top:106px;width:960px;height:189px"></div>
<div class="gt" style="left:39px;top:107.7px">Personas dati</div>
<div class="lb " style="left:-140px;top:139.9px;width:300px;text-align:right">Personas kods</div>
<div class="lb " style="left:-140px;top:171.9px;width:300px;text-align:right">Uzvārds</div>
<div class="lb " style="left:-140px;top:203.9px;width:300px;text-align:right">Vārds (i)</div>
<div class="lb " style="left:-140px;top:235.9px;width:300px;text-align:right">Dzimums</div>
<input id="s2-kods" class="f gr" style="left:163px;top:141px;width:170px;height:21px" value="" readonly tabindex="-1" placeholder="Tiks ģenerēts" autocomplete="off" spellcheck="false">
<input id="s2-uzv" class="f cy" style="left:163px;top:173px;width:330px;height:21px" value="BERZINS" autocomplete="off" spellcheck="false">
<input id="s2-vards" class="f cy" style="left:163px;top:205px;width:330px;height:21px" value="JANIS" autocomplete="off" spellcheck="false">
<input id="s2-dzim" class="f cy" style="left:163px;top:237px;width:60px;height:21px" value="V" maxlength="1" autocomplete="off" spellcheck="false">
<div class="lb " style="left:380px;top:139.9px;width:300px;text-align:right">Dzimšanas datums</div>
<div class="lb " style="left:380px;top:171.9px;width:300px;text-align:right">Miršanas datums</div>
<div class="lb " style="left:380px;top:203.9px;width:300px;text-align:right">Valsts</div>
<div class="lb " style="left:380px;top:235.9px;width:300px;text-align:right">Pilsonība</div>
<input id="s2-dzd" class="f cy" style="left:683px;top:141px;width:110px;height:21px" value="11.11.1911" autocomplete="off" spellcheck="false">
<input id="s2-mird" class="f cy" style="left:683px;top:173px;width:110px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-valsts" class="f cy" style="left:683px;top:205px;width:250px;height:21px" value="BULGĀRIJA" autocomplete="off" spellcheck="false">
<input id="s2-pils" class="f cy" style="left:683px;top:237px;width:250px;height:21px" value="" autocomplete="off" spellcheck="false">
<div class="grp" style="left:7px;top:302px;width:590px;height:153px"></div>
<div class="gt" style="left:39px;top:304.7px">Identifikācijas kodi</div>
<div class="lb " style="left:26px;top:325.29999999999995px;width:300px;text-align:left">Identifikācijas kods</div>
<div class="lb " style="left:154px;top:325.29999999999995px;width:300px;text-align:left">Valsts</div>
<div class="lb " style="left:255px;top:325.29999999999995px;width:300px;text-align:left">Organizācija</div>
<input id="s2-k0a" class="f cy" style="left:25px;top:340px;width:127px;height:21px" value="1234-5678" autocomplete="off" spellcheck="false">
<input id="s2-k0b" class="f cy" style="left:153px;top:340px;width:100px;height:21px" value="BULGĀRIJA" autocomplete="off" spellcheck="false">
<input id="s2-k0c" class="f cy" style="left:254px;top:340px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k1a" class="f cy" style="left:25px;top:362px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k1b" class="f cy" style="left:153px;top:362px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k1c" class="f cy" style="left:254px;top:362px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k2a" class="f cy" style="left:25px;top:383px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k2b" class="f cy" style="left:153px;top:383px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k2c" class="f cy" style="left:254px;top:383px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k3a" class="f cy" style="left:25px;top:405px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k3b" class="f cy" style="left:153px;top:405px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k3c" class="f cy" style="left:254px;top:405px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k4a" class="f cy" style="left:25px;top:426px;width:127px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k4b" class="f cy" style="left:153px;top:426px;width:100px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-k4c" class="f cy" style="left:254px;top:426px;width:307px;height:21px" value="" autocomplete="off" spellcheck="false">
<div class="sb" style="left:562px;top:340px;width:14px;height:108px"><i class="up"></i><i class="dn"></i><b></b></div>
<div class="grp" style="left:605px;top:340px;width:338px;height:119px"></div>
<div class="gt" style="left:637px;top:342.7px">Adrese</div>
<div class="lb " style="left:409px;top:366.9px;width:300px;text-align:right">Valsts</div>
<div class="lb " style="left:409px;top:387.9px;width:300px;text-align:right">Pilsēta/rajons</div>
<div class="lb " style="left:409px;top:409.9px;width:300px;text-align:right">Iela/māja</div>
<div class="lb " style="left:409px;top:429.9px;width:300px;text-align:right">Pasta indekss</div>
<input id="s2-a0" class="f cy" style="left:710px;top:363px;width:211px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-a1" class="f cy" style="left:710px;top:384px;width:211px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-a2" class="f cy" style="left:710px;top:406px;width:211px;height:21px" value="" autocomplete="off" spellcheck="false">
<input id="s2-a3" class="f cy" style="left:710px;top:427px;width:187px;height:21px" value="" autocomplete="off" spellcheck="false">
<button type="button" id="s2-reg" class="btn " style="left:727px;top:480px;width:163px;height:31px">Reģistrēt</button>
<button type="button" id="s2-atc" class="btn " style="left:900px;top:480px;width:100px;height:31px">Atcelt</button>
<div class="dlg" id="s2-dlg" hidden><div class="dh">SAIS</div><div class="dm" id="s2-dm"></div><button type="button" class="btn" id="s2-ok" style="left:110px;top:90px;width:80px;height:26px">Labi</button></div><div class="bb"></div></form>
</div>
<p class="note">Prototips. Spiediet "Reģistrēt jaunu personu SAIS", lai atvērtu reģistrācijas formu. Lauku saturs ir piemērs no SED dokumenta; personas koda formāts ir ilustratīvs.</p>
<script>
(function(){
  var s1=document.getElementById('s1'),s2=document.getElementById('s2');
  var dlg=document.getElementById('s2-dlg'),dm=document.getElementById('s2-dm');
  function $(id){return document.getElementById(id)}
  $('s1-regnew').addEventListener('click',function(){s1.hidden=true;s2.hidden=false;dlg.hidden=true;$('s2-uzv').focus()});
  function back(){s2.hidden=true;s1.hidden=false;dlg.hidden=true;
    Array.prototype.forEach.call(s2.querySelectorAll('input'),function(e){e.disabled=false;e.classList.remove('bad')});$('s2-reg').disabled=false}
  $('s2-atc').addEventListener('click',back);
  function vd(s){var m=/^(\d{2})\.(\d{2})\.(\d{4})$/.exec(s.trim());if(!m)return false;var d=new Date(+m[3],+m[2]-1,+m[1]);return d.getFullYear()==+m[3]&&d.getMonth()==+m[2]-1&&d.getDate()==+m[1]}
  function show(t){dm.textContent=t;dlg.hidden=false}
  $('s2-reg').addEventListener('click',function(){
    var bad=[];
    ['uzv','vards','dzim','dzd','valsts'].forEach(function(id){var e=$('s2-'+id),v=e.value.trim();var ok=v&&(id!=='dzd'||vd(v))&&(id!=='dzim'||/^[VvSs]$/.test(v));e.classList.toggle('bad',!ok);if(!ok)bad.push(e)});
    var m=$('s2-mird'),mok=!m.value.trim()||vd(m.value);m.classList.toggle('bad',!mok);if(!mok)bad.push(m);
    if(bad.length){show('Aizpildiet obligātos laukus: uzvārds, vārds, dzimums (V/S), dzimšanas datums (DD.MM.GGGG), valsts.');bad[0].focus();return}
    var n=function(k){var s='';for(var i=0;i<k;i++)s+=Math.floor(Math.random()*10);return s};
    var code=n(6)+'-'+n(5);
    $('s2-kods').value=code;
    Array.prototype.forEach.call(s2.querySelectorAll('input'),function(e){e.disabled=true});$('s2-reg').disabled=true;
    show('Persona reģistrēta SAIS ar kodu '+code+'. Pamatojošais dokuments: SED lieta 3570. Persona sasaistīta ar SED personu.');
  });
  $('s2-ok').addEventListener('click',function(){dlg.hidden=true;if($('s2-reg').disabled){
    var c=$('s2-kods').value;back();$('s1-pkods').value=c;$('s1-pvards').value=$('s2-vards').value;$('s1-puzv').value=$('s2-uzv').value;
  }});
})();
</script>
</body>
</html>
