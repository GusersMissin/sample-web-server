# sample-web-server
テクノロジー（藤原）Node.jsによるサンプルWebサーバ

```
cd fujiwara/
(base) Ans-MacBook-Pro:fujiwara missingusers$ ls
hello-git        learning-http-message    simple-web-site
(base) Ans-MacBook-Pro:fujiwara missingusers$ git clone git@github.com:GusersMissin/sample-web-server.git
Cloning into 'sample-web-server'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 7 (delta 1), reused 5 (delta 1), pack-reused 0
Receiving objects: 100% (7/7), done.
Resolving deltas: 100% (1/1), done.
(base) Ans-MacBook-Pro:fujiwara missingusers$ cd sample-web-server/
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl --silent --request GET --url https://api.thecatapi.com/v1/images/search
[{"breeds":[],"id":"a0i","url":"https://cdn2.thecatapi.com/images/a0i.jpg","width":500,"height":332}](base) Ans-MacBook-Pro:sample-web-server missingusers$ curlET --url "https://api.thecatapi.com/v1/images/search?limit=3'
> ;
> '
> ;
> ;
> 
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3'
[{"breeds":[],"id":"8er","url":"https://cdn2.thecatapi.com/images/8er.jpg","width":500,"height":462},{"breeds":[],"id":"b03","url":"https://cdn2.thecatapi.com/images/b03.jpg","width":500,"height":334},{"breeds":[],"id":"MTYyNDcyOA","url":"https://cdn2.thecatapi.com/images/MTYyNDcyOA.jpg","width":2448,"height":3264}](base) Ans-MacBook-Pro:sample-web-server missingusers$ brew install jq
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> New Formulae
cjson                                    procs
clojure-lsp                              scala@2.12
docker-machine-driver-vmware             scdoc
drone-cli                                swig@3
dust                                     termshark
hey                                      terraformer
ipopt                                    virgil
newman
==> Updated Formulae
curl-openssl ✔                           kubernetes-service-catalog-client
glib ✔                                   lasi
libev ✔                                  latex2html
openssl ✔                                ledger
phpmyadmin ✔                             lgogdownloader
akamai                                   libbitcoin
angular-cli                              libbitcoin-blockchain
ansible                                  libbitcoin-client
anyenv                                   libbitcoin-database
arangodb                                 libbitcoin-explorer
aravis                                   libbitcoin-network
armadillo                                libbitcoin-node
ask-cli                                  libbitcoin-protocol
atlantis                                 libbitcoin-server
autorest                                 libical
avro-cpp                                 libosinfo
aws-sdk-cpp                              libpulsar
azure-cli                                librealsense
azure-storage-cpp                        libsigc++
bazel                                    libswiften
bit                                      libtorrent-rasterbar
bitcoin                                  libvirt
bitrise                                  linkerd
bitwarden-cli                            lmod
boost                                    macvim
boost-bcp                                mame
boost-build                              mariadb-connector-c
boost-mpi                                maxima
boost-python                             mercurial
boost-python3                            mesa
braid                                    metaproxy
buildifier                               micronaut
caffe                                    mighttpd2
calicoctl                                minio
certbot                                  minio-mc
cfn-lint                                 mk-configure
cgal                                     mksh
chakra                                   mkvtoolnix
circleci                                 molecule
citus                                    monero
clojure                                  monetdb
cointop                                  mpich
composer                                 nativefier
conan                                    nats-streaming-server
convox                                   ncmpcpp
cpprestsdk                               nim
cromwell                                 node
cryfs                                    node-build
crystal                                  node_exporter
cucumber-cpp                             nomad
curl                                     opa
cython                                   openimageio
deno                                     osquery
dependency-check                         osrm-backend
dhall                                    paket
django-completion                        pam-u2f
dnscrypt-proxy                           pandoc
doctl                                    pgrouting
duck                                     php-cs-fixer
duo_unix                                 phpunit
encfs                                    pod2man
envconsul                                pre-commit
erlang                                   prettier
erlang@21                                proteinortho
exiftool                                 prototool
exploitdb                                pstoedit
firebase-cli                             pulumi
flow                                     pybind11
fluxctl                                  pyenv
fn                                       quicktype
folly                                    rbspy
fontforge                                rke
fselect                                  scala
fuseki                                   scalariform
futhark                                  scons
gdcm                                     scrcpy
gengetopt                                serverless
geoipupdate                              sfcgal
gibo                                     shadowsocks-libev
git                                      ship
git-remote-hg                            skaffold
gitlab-runner                            solr@7.7
gitleaks                                 sops
glib-networking                          source-highlight
glooctl                                  sphinx-doc
gmic                                     sslsplit
gnu-units                                telegraf
gnumeric                                 terraform
gnunet                                   terragrunt
gnuradio                                 terrahub
go                                       tfenv
godep                                    thefuck
goffice                                  tile38
golang-migrate                           tokei
goofys                                   tomcat
goreleaser                               topgrade
gpsbabel                                 tox
grafana                                  u-boot-tools
grakn                                    uhd
graph-tool                               upscaledb
grpc                                     v8
gst-plugins-good                         vala
helmfile                                 vault
hlint                                    vim
hyperfine                                vultr
i2pd                                     webpack
icecream                                 weechat
imagemagick                              wesnoth
imagemagick@6                            whois
inlets                                   widelands
istioctl                                 wildfly-as
itk                                      wimlib
jdupes                                   wtf
jenkins                                  xonsh
jenkins-lts                              yamllint
jfrog-cli-go                             yelp-tools
jhipster                                 ykman
joplin                                   you-get
juju                                     youtube-dl
knot                                     yubico-piv-tool
kubernetes-cli                           zim
kubernetes-helm                          zlog
==> Renamed Formulae
gnatsd -> nats-server
==> Deleted Formulae
scala@2.10                               swig@3.04

==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bott
==> Downloading from https://akamai.bintray.com/c6/c613befafe81da48913ebd1a7eb03
######################################################################## 100.0%
==> Pouring oniguruma-6.9.2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/oniguruma/6.9.2: 17 files, 1.3MB
==> Installing jq
==> Downloading https://homebrew.bintray.com/bottles/jq-1.6.mojave.bottle.1.tar.
==> Downloading from https://akamai.bintray.com/71/71f0e76c5b22e5088426c971d5e79
######################################################################## 100.0%
==> Pouring jq-1.6.mojave.bottle.1.tar.gz
🍺  /usr/local/Cellar/jq/1.6: 18 files, 1MB
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl --silent --request 'https://api.thecatapi.com/v1/images/search?limit=3' | jq
curl: no URL specified!
curl: try 'curl --help' or 'curl --manual' for more information
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl --silent --request GET 'https://api.thecatapi.com/v1/images/search?limit=3' | jq
[
{
"breeds": [],
"id": "24d",
"url": "https://cdn2.thecatapi.com/images/24d.jpg",
"width": 500,
"height": 333
},
{
"breeds": [],
"id": "ae3",
"url": "https://cdn2.thecatapi.com/images/ae3.gif",
"width": 500,
"height": 214
},
{
"breeds": [
{
"weight": {
"imperial": "6 - 14",
"metric": "3 - 6"
},
"id": "emau",
"name": "Egyptian Mau",
"cfa_url": "http://cfa.org/Breeds/BreedsCJ/EgyptianMau.aspx",
"vetstreet_url": "http://www.vetstreet.com/cats/egyptian-mau",
"vcahospitals_url": "https://vcahospitals.com/know-your-pet/cat-breeds/egyptian-mau",
"temperament": "Agile, Dependent, Gentle, Intelligent, Lively, Loyal, Playful",
"origin": "Egypt",
"country_codes": "EG",
"country_code": "EG",
"description": "The Egyptian Mau is gentle and reserved. She loves her people and desires attention and affection from them but is wary of others. Early, continuing socialization is essential with this sensitive and sometimes shy cat, especially if you plan to show or travel with her. Otherwise, she can be easily startled by unexpected noises or events.",
"life_span": "18 - 20",
"indoor": 0,
"lap": 1,
"alt_names": "Pharaoh Cat",
"adaptability": 2,
"affection_level": 5,
"child_friendly": 3,
"dog_friendly": 3,
"energy_level": 5,
"grooming": 1,
"health_issues": 3,
"intelligence": 4,
"shedding_level": 3,
"social_needs": 4,
"stranger_friendly": 2,
"vocalisation": 3,
"experimental": 0,
"hairless": 0,
"natural": 1,
"rare": 0,
"rex": 0,
"suppressed_tail": 0,
"short_legs": 0,
"wikipedia_url": "https://en.wikipedia.org/wiki/Egyptian_Mau",
"hypoallergenic": 0
}
],
"id": "BZ59tdOo6",
"url": "https://cdn2.thecatapi.com/images/BZ59tdOo6.jpg",
"width": 1280,
"height": 720
}
]
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
(base) Ans-MacBook-Pro:sample-web-server missingusers$ cat ~/.bash_profile

# Setting PATH for Python 2.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/2.7/bin:${PATH}"
export PATH

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
# added by Anaconda2 2019.03 installer
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/anaconda2/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
\eval "$__conda_setup"
else
if [ -f "/anaconda2/etc/profile.d/conda.sh" ]; then
. "/anaconda2/etc/profile.d/conda.sh"
CONDA_CHANGEPS1=false conda activate base
else
\export PATH="/anaconda2/bin:$PATH"
fi
fi
unset __conda_setup
# <<< conda init <<<
# added by Anaconda3 2019.03 installer
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/anaconda3/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
\eval "$__conda_setup"
else
if [ -f "/anaconda3/etc/profile.d/conda.sh" ]; then
. "/anaconda3/etc/profile.d/conda.sh"
CONDA_CHANGEPS1=false conda activate base
else
\export PATH="/anaconda3/bin:$PATH"
fi
fi
unset __conda_setup
# <<< conda init <<<
(base) Ans-MacBook-Pro:sample-web-server missingusers$ echo "if [ -f ~/.bashrc ]; then" >> ~/.bash_profile
(base) Ans-MacBook-Pro:sample-web-server missingusers$ echo " . ~/.bashrc" >> ~/.bash_profile
(base) Ans-MacBook-Pro:sample-web-server missingusers$ echo "fi" >> ~/.bash_profile
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl -L git.io/nodebrew | perl -setup
% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
Dload  Upload   Total   Spent    Left  Speed
0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0
0     0    0     0    0     0      0      0 --:--:--  0:00:03 --:--:--     0
74 24634   74 18301    0     0   5123      0  0:00:04  0:00:03  0:00:01  5123
curl: (23) Failed writing body (0 != 2759)
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl -L git.io/nodebrew | perl -setup
% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
Dload  Upload   Total   Spent    Left  Speed
0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
0     0    0     0    0     0      0      0 --:--:--  0:00:03 --:--:--     0
74 24634   74 18303    0     0   5445      0  0:00:04  0:00:03  0:00:01  5445
curl: (23) Failed writing body (0 != 2759)
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl -L git.io/nodebrew | perl - setup
% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
Dload  Upload   Total   Spent    Left  Speed
0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0
0     0    0     0    0     0      0      0 --:--:--  0:00:03 --:--:--     0
100 24634  100 24634    0     0   7860      0  0:00:03  0:00:03 --:--:--  279k
Fetching nodebrew...
Installed nodebrew in $HOME/.nodebrew

========================================
Export a path to nodebrew:

export PATH=$HOME/.nodebrew/current/bin:$PATH
========================================
(base) Ans-MacBook-Pro:sample-web-server missingusers$ export PATH=$HOME/.nodebrew/current/bin:$PATH >> ~/.bashrc
(base) Ans-MacBook-Pro:sample-web-server missingusers$ source ~/.bashrc
(base) Ans-MacBook-Pro:sample-web-server missingusers$ nodebrew
nodebrew 1.0.1

Usage:
nodebrew help                         Show this message
nodebrew install <version>            Download and install <version> (from binary)
nodebrew compile <version>            Download and install <version> (from source)
nodebrew install-binary <version>     Alias of `install` (For backward compatibility)
nodebrew uninstall <version>          Uninstall <version>
nodebrew use <version>                Use <version>
nodebrew list                         List installed versions
nodebrew ls                           Alias for `list`
nodebrew ls-remote                    List remote versions
nodebrew ls-all                       List remote and installed versions
nodebrew alias <key> <value>          Set alias
nodebrew unalias <key>                Remove alias
nodebrew clean <version> | all        Remove source file
nodebrew selfupdate                   Update nodebrew
nodebrew migrate-package <version>    Install global NPM packages contained in <version> to current version
nodebrew exec <version> -- <command>  Execute <command> using specified <version>

Example:
# install
nodebrew install v8.9.4

# use a specific version number
nodebrew use v8.9.4
(base) Ans-MacBook-Pro:sample-web-server missingusers$ nodebrew install-binary latest
Fetching: https://nodejs.org/dist/v12.4.0/node-v12.4.0-darwin-x64.tar.gz
#######                                                                    10.0%^Cdownload failed: https://nodejs.org/dist/v12.4.0/node-v12.4.0-darwin-x64.tar.gz
(base) Ans-MacBook-Pro:sample-web-server missingusers$ nodebrew install-binary latest
Fetching: https://nodejs.org/dist/v12.4.0/node-v12.4.0-darwin-x64.tar.gz
######################################################################### 100.0%
Installed successfully
(base) Ans-MacBook-Pro:sample-web-server missingusers$ nodebrew ls
v12.4.0

current: none
(base) Ans-MacBook-Pro:sample-web-server missingusers$ nodebrew use latest
use v12.4.0
(base) Ans-MacBook-Pro:sample-web-server missingusers$ node -v
v12.4.0
(base) Ans-MacBook-Pro:sample-web-server missingusers$ curl --silent --request GET --url https://api.thecatapi.com/v1/images/search
[{"breeds":[],"id":"cko","url":"https://cdn2.thecatapi.com/images/cko.jpg","width":1280,"height":960}](base) Ans-MacBook-Pro:sample-web-server missingusers$ ls
README.md    thecat.json
(base) Ans-MacBook-Pro:sample-web-server missingusers$ mkdir mywebapi
(base) Ans-MacBook-Pro:sample-web-server missingusers$ cd mywebapi/
(base) Ans-MacBook-Pro:mywebapi missingusers$ npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
package name: (mywebapi) 
version: (1.0.0) 
description: 
entry point: (index.js) 
test command: 
git repository: 
keywords: 
author: 
license: (ISC) 
About to write to /Users/missingusers/Desktop/01授業資料/01テクノロジー/03藤原先生/fujiwara/sample-web-server/mywebapi/package.json:

{
"name": "mywebapi",
"version": "1.0.0",
"description": "",
"main": "index.js",
"scripts": {
"test": "echo \"Error: no test specified\" && exit 1"
},
"author": "",
"license": "ISC"
}


Is this OK? (yes) yes
(base) Ans-MacBook-Pro:mywebapi missingusers$ npm install --save express
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN mywebapi@1.0.0 No description
npm WARN mywebapi@1.0.0 No repository field.

+ express@4.17.1
added 50 packages from 37 contributors and audited 126 packages in 3.527s
found 0 vulnerabilities

(base) Ans-MacBook-Pro:mywebapi missingusers$ ls
node_modules        package-lock.json    package.json
(base) Ans-MacBook-Pro:mywebapi missingusers$ vi index.js
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js
/Users/missingusers/Desktop/01授業資料/01テクノロジー/03藤原先生/fujiwara/sample-web-server/mywebapi/index.js:4
app.listen(3000,()=>console.log('Listening on port 3000')):
^

SyntaxError: Unexpected token :
at Module._compile (internal/modules/cjs/loader.js:718:23)
at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
at Module.load (internal/modules/cjs/loader.js:641:32)
at Function.Module._load (internal/modules/cjs/loader.js:556:12)
at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
at internal/main/run_main_module.js:17:11
(base) Ans-MacBook-Pro:mywebapi missingusers$ vi index.js
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js 
Listening on port 3000
^C
(base) Ans-MacBook-Pro:mywebapi missingusers$ vi index.js 
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js
Listening on port 3000
^C
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js 
Listening on port 3000
^C
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js
/Users/missingusers/Desktop/01授業資料/01テクノロジー/03藤原先生/fujiwara/sample-web-server/mywebapi/index.js:3
app.arguments(express.static('web'));
^

TypeError: 'caller', 'callee', and 'arguments' properties may not be accessed on strict mode functions or the arguments objects for calls to them
at Object.<anonymous> (/Users/missingusers/Desktop/01授業資料/01テクノロジー/03藤原先生/fujiwara/sample-web-server/mywebapi/index.js:3:5)
at Module._compile (internal/modules/cjs/loader.js:774:30)
at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
at Module.load (internal/modules/cjs/loader.js:641:32)
at Function.Module._load (internal/modules/cjs/loader.js:556:12)
at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
at internal/main/run_main_module.js:17:11
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js
/Users/missingusers/Desktop/01授業資料/01テクノロジー/03藤原先生/fujiwara/sample-web-server/mywebapi/index.js:3
app.arguments(express.static('web'));
^

TypeError: 'caller', 'callee', and 'arguments' properties may not be accessed on strict mode functions or the arguments objects for calls to them
at Object.<anonymous> (/Users/missingusers/Desktop/01授業資料/01テクノロジー/03藤原先生/fujiwara/sample-web-server/mywebapi/index.js:3:5)
at Module._compile (internal/modules/cjs/loader.js:774:30)
at Object.Module._extensions..js (internal/modules/cjs/loader.js:785:10)
at Module.load (internal/modules/cjs/loader.js:641:32)
at Function.Module._load (internal/modules/cjs/loader.js:556:12)
at Function.Module.runMain (internal/modules/cjs/loader.js:837:10)
at internal/main/run_main_module.js:17:11
(base) Ans-MacBook-Pro:mywebapi missingusers$ node index.js
Listening on port 3000
^C
^C
(base) Ans-MacBook-Pro:mywebapi missingusers$ 
(base) Ans-MacBook-Pro:mywebapi missingusers$ npm install --save multer uuid
npm WARN mywebapi@1.0.0 No description
npm WARN mywebapi@1.0.0 No repository field.

+ multer@1.4.1
+ uuid@3.3.2
added 22 packages from 18 contributors and audited 165 packages in 2.737s
found 0 vulnerabilities

```
