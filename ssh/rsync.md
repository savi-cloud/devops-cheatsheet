### This to Destination
rsync -a ~/dir1 username@remote_host:destination_directory

### Remote to this
rsync -a username@remote_host:/home/username/dir1 place_to_sync_on_local_machine


### Define Key
rsync -Pav -e "ssh -i $HOME/.ssh/somekey" username@hostname:/from/dir/ /to/dir/

### Exclue
rsync -a --exclude 'dir1' src_directory/ dst_directory/

https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories