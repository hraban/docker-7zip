## Dockerized 7zip


### Examples

Add Oracle folder to test1.7z:

    docker run -it --rm -v $(pwd):/pwd -w /pwd luyat/7zip 7zip a test1 Oracle

Use tar to preserve UNIX permissions and ownership:

    docker run -ti --rm -v "$PWD:/pwd" -w /pwd luyat/7zip bash -c 'tar c Oracle | 7z a -si test1.tar.7z'

