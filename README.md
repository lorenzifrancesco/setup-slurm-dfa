# setup-slurm-dfa
Collection of useful tools and methods for the setup of a SLURM computing system for scientific research 

## Setup the VM on CloudVeneto

Tunnel to Cloudveneto, with command 
```bash 
cloudveneto_tunnel="ssh -L2080:10.64.37.31:22 florenzi@gate.cloudveneto.it"
```

gives access to shell and to the shared folders

```bash
florenzi@gate.cloudveneto.it's password: 
Last failed login: Tue Nov 14 19:31:02 CET 2023 from 73.red-79-153-55.dynamicip.rima-tde.net on ssh:notty
There were 3 failed login attempts since the last successful login.
Last login: Wed Oct  4 09:48:31 2023 from 147.83.54.95
bash-4.2$ 
bash-4.2$ lscpu
bash: lscpu: command not found
bash-4.2$ whoami
bash: whoami: command not found
bash-4.2$ ls
bash-4.2$ cd /
bash-4.2$ ll
bash: ll: command not found
bash-4.2$ s
bash: s: command not found
bash-4.2$ ls
bin  dev  etc  home  lib64  usr
bash-4.2$ cd home
bash-4.2$ ls
aanilkum  alorenzo   atriossi	collamaf	  dpiccoli	  erbucalo  fmenegaz	gbrunell  haweber   lacaprar	lvdauria	   mdedomen  mmorgavi  orsinife   ronca		     slibanor	 vbedin
aarzento  amarchet   atroja	collazuo	  drattaca	  ereniero  fnardi	gcalajo   hluciani  laportas	lvedovel	   mdib      mnaimoli  parim	  ronchese	     slipani	 vbettio
aattar	  amollaal   atrovato	comunian	  drisso	  erodrigu  forlando	gcalvino  hmunch    lbarbiero	lzago		   mdiliber  mpadovan  passera	  rrajaee	     smoro	 vcerrone
abasiric  amomtaz    avalsecc	cpjowen		  drodermu	  erossi    fpassal	gcataldi  igiovann  lcaldera	lzampier	   mdoro     mpagin    pavanello  rrossin	     smunafo	 vitella
abegnoni  amontell   azal	csgorlon	  dserafin	  esarte    fpicano	gcelotto  igrimald  lcrema	mallegra	   mdrago    mpegorin  pazzini	  rtancred	     snotarni	 vmarrali
abianchi  anambena   azanoli	ctestini	  dsorokin	  etoffali  fpicciar	gcrisant  isiloi    lfilotto	malraham	   melkhash  mperon    pbernard   rturrisi	     spacheco	 vonsturm
abraghet  anamvar    azucchet	cverones	  dusini	  evanzan   fpirotti	gdiprima  istankov  lfinos	mamandal	   menego    mpihet    pertoldi   saboud	     sscaltri	 wwaththe
abreccia  apaccagn   batkovic	cvorsman	  dzanchet	  ezoppell  fpraflor	ggzhang   iviale    lgabarra	marcased	   mfeizi    mpvvatin  pgrutta	  sahsanin	     ssepehri	 xizhang
abriscio  apatelli   bazzacco	dallagat	  dzuliani	  fancilot  frecchia	gianelle  jacksonj  lgiambas	marchiori	   mferrari  mqasim    pmajcen	  samir.suweis	     sstalio	 xwu
acacioll  apietrac   bcruzmae	daltamir	  eahmadie	  fantinel  fromanat	gibin	  jakkara   lgiammor	marco.dallatiezza  mferrazz  mrigobel  pmastrap   sanazbar	     stoppo	 ylashko
acapodag  apitteri   bdecaro	damiano.falcioni  ebaci		  fapasian  fruffini	ginverso  jbenito   lgiorget	margoni		   mfuxreit  mroccatt  pmiglior   sanselmi	     storniam	 ymascolo
acarraro  apolimen   bellanl	dbacilieri	  ebalzani	  farnese   fsantoli	giorio	  jderivau  lgrassi	martale		   mgholami  mroshana  ppadmana   sanzules	     stoso	 yong
acoppi	  apozzobon  bertolin	dbanerje	  ebatzell	  fbaghaei  fsemenza	gisotton  jkandra   liguorim	mascagna	   mgiacchi  msaeedia  ppoli	  sbabakha	     stroili	 ypervysh
acostant  arangraz   bgatto	dbarone		  ebazzani	  fballout  fsimonat	gmagnifi  jmarino   lippi	mavesani	   mgrassi   msapkas   prandini   scampese	     svasiuko	 ypu
adainese  aravenni   biasotto	dbenussi	  ebrisigo	  fbarbaro  fsimpsi	gmerlin   jmazzon   llitti	mbaiesi		   mgravino  mseppi    psala	  scarollo	     syadav	 zumerle
adebei	  arenzi     bjelmini	dbernard	  echueva	  fbarone   fspezzat	gmoretti  jnauta    lmancini	mbarbieri	   mhergnya  mtesoro   pumari	  scavinat	     taffarel
adevita   arezzi     bredo	dbonato		  eeslamis	  fborgato  fulvia	gnagaroq  jniederm  lmattiaz	mbassoli	   micetic   mtessaro  pupillif   scuencal	     tbertape
adisarci  aricciar   brugnera	dchecchi	  efella	  fbraidi   fulvia.old	gnicolet  jpacheco  lmengoni	mbellato	   micromed  mtosi     pwickram   sdinoi	     tbertola
adoimo	  arossi     buoninco	dchen		  egonzale	  fcampaio  fzambell	goasduff  jpadilla  lmenti	mboscato	   mkeshava  mvaccaro  pzinesi	  sdubey	     tcaba
afeltrin  arostami   caime	ddefranc	  eleonell	  fcassol   fzane	gperna	  jpasqual  longhin	mbruschi	   mlanaro   mvatankh  qzhang	  selsasan	     tdorigo
aferaru   aruina     canton	degrandis	  elocatel	  fcima     fzanetti	gricucci  jpchryss  loris	mcacciol	   mlunardo  mzanetti  rardino	  sestini	     tguercio
aforoni   asaccoma   cantonio	delazzar	  elongato	  fdallaba  gaggio	gsaielli  jramosda  lotti	mcaldera	   mmariott  mzenari   rbhatti	  sgaraprova	     tmarchi
agarbo	  ascapola   carcaro	dfaggin		  elupi		  ffagosti  gandreet	gsardoin  jskowron  lsaccaro	mcampore	   mmattiaz  nargiola  rceccato   sghaemif	     tolbatov
agarfa	  aselva     ccorrido	dhjordan	  elusiani	  ffesta    gbaltaba	gsciacca  jtorrado  lsalicar	mcasarsa	   mmattius  nbee      rdezen	  sgiustin	     torassa
agavriko  aserafin   ccuratol	djaschke	  emariott	  ffischer  gbarzon	gsilvest  jverguiz  lsanavia	mcastell	   mmeneghe  nlai      rebeccani  sgugliel	     tosatto
agaz	  ashojaei   cdivari	dmarcato	  emomeni	  fgonella  gbertin	gstrong   jvinesse  lspina	mcavazza	   mmerola   nmanara   rfiorott   shoof		     tpasupat
agozzeli  aspolon    cforza	dmarches	  enzo.orlandini  florenzi  gbertine	gulmini   karoonru  luca_maran	mceccare	   mmiglior  nmuhamma  rgolan	  silvestri	     traforetti
aguilera  aspoto     chanasorn	dmiceli		  epeseric	  fmambret  gbezze	gverza	  kjavid    lucchesi	mchiloir	   mmiranda  nsahputr  rigoni	  simi		     tscaglia
aleoncas  atestoli   checchia	dninni		  epigani	  fmarzari  gbonomi	gviterbo  kpanagio  lupato	mcogo		   mmontis   nselimov  rlenzo	  simo		     ttasneem
aleso	  atonon     chestnov	dpanarit	  equaglio	  fmazza    gbordin	gzago	  ktrawall  lvalenti	mdallara	   mmorandi  nzomer    rlopez	  simone.montangero  uhasret
```

Access to the VM is then obtained via 

```bash
cloudveneto_shell="ssh -p 2080 -i ~/.ssh/certificates/Lorenzi.pem ubuntu@localhost"
```

connections in local tunnel ports 2080 (login) and 2081 (slurPh).

Installation of SLURM is then performed following the instructions at

> https://github.com/PKUHPC/slurm-deployment/blob/main/How%20to%20Install%20Slurm%20on%20CentOS%207%20Cluster.md

## Install SLURM
the dependencies can be installed via the PowerTools repo, that is accessible via ```dnf```.

The RPM install got errors 
```bash
RPM build errors:
    Macro expanded in comment on line 22: %_prefix path		install path for commands, libraries, etc.

    Macro expanded in comment on line 30: %_with_hwloc 1		require hwloc support

    Macro expanded in comment on line 31: %_with_lua path		build Slurm lua bindings

    Macro expanded in comment on line 185: %define _unpackaged_files_terminate_build      0

    Empty %files file /root/rpmbuild/BUILD/slurm-23.02.6/slurm.files
    File not found: /root/rpmbuild/BUILDROOT/slurm-23.02.6-1.el8.x86_64/usr/lib64/slurm/accounting_storage_mysql.so
    File listed twice: /usr/lib/.build-id/64/e2828b53a14c5f883b6e4ca821356d9f749e6c
    File listed twice: /usr/lib/.build-id/66/f24a5d908892f21911e0a6cf82d23c5e8c1cfd
    File listed twice: /usr/lib/.build-id/68/c936ad4b0308cfa5fbc890358dce82be9d222f
    File listed twice: /usr/lib/.build-id/8d/354fab9448a4e69a6088c21600d38799456731
    Deprecated external dependency generator is used!
    Deprecated external dependency generator is used!
    Deprecated external dependency generator is used!
    Empty %files file /root/rpmbuild/BUILD/slurm-23.02.6/example.configs
    Deprecated external dependency generator is used!
    Deprecated external dependency generator is used!
    Deprecated external dependency generator is used!
    File not found: /root/rpmbuild/BUILDROOT/slurm-23.02.6-1.el8.x86_64/usr/lib64/slurm/accounting_storage_mysql.so
```