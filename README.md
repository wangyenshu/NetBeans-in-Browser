NetBeans in Browser

Screenshot:
![screenshot](screenshot.png)
How to build:

- clone this project
- run `cd tools/docker/NetBeans`
- run 'wget https://archive.apache.org/dist/netbeans/netbeans/12.6/netbeans-12.6-bin.zip'
- run `./build.sh`
- run `./build-state.js`
- run 'cp split.sh ../../../images/split.sh'
- run `cd ../../../images`
- run './split.sh'
- run 'rm debian-9p-rootfs.tar debian-state-base.bin'
- run 'cd ..'
- run `make run`

  This should start a server on 8000 (or other ports).

Credit:
- Apache NetBeans: https://netbeans.apache.org/front/main/about/
- Apache NetBeans License: https://www.apache.org/licenses/LICENSE-2.0
- v86: https://github.com/copy/v86
- sandbox.bio's debian 12 on v86 configuration: https://github.com/sandbox-bio/v86
