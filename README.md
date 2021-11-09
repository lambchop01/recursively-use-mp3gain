# recursively-use-mp3gain

install mp3 gain
1. sudo add-apt-repository ppa:flexiondotorg/audio
2. sudo apt-get install mp3gain

options -> https://www.mankier.com/1/mp3gain

bash command to recursively treat each folder as an album.
`find ./ -type d -exec bash -c 'cd "$1"; mp3gain -a -k -p *.mp3' -- {} \;`
