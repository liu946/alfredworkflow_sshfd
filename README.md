sshfs.alfredworkflow
---

To mount your remote disk using ssh protocal.

## Run

1. Launch your Alfred, type `sshfs`, select the server to mount.

![alfred](https://github.com/liu946/alfredworkflow_sshfd/blob/master/doc/alfred.png?raw=true)

2. Access your remote file at 'finder' locally.

![finder](https://github.com/liu946/alfredworkflow_sshfd/blob/master/doc/finder.png?raw=true)

## Installation

1. Make sure you have installed [Alfred](https://www.alfredapp.com/) and you can use the [Powerpack](https://www.alfredapp.com/powerpack/buy/).
2. Download the workflow package
3. Double click the sshfs.alfredworkflow or drag it into Alfred Preference -> Workflows.
4. Install `sshfs` (using `brew`, `apt-get`, `yum`, whatever...) and find it's absolute path (for me it is `/usr/local/bin/sshfs`)
5. Double click the square which has a cloud-disk icon on it and rewrite the `SSHFS_PATH='/usr/local/bin/sshfs'` to your path in step 4.
6. Rewrite the variable `RemoteDisk` by all your remote servers (you can login on them with sshkey without password) then save. You can refer the format as below.

```
RemoteDisk=(
	<name for show> <ip/url> <remote username> <port> <remote path being mapped> <local path to be mapped to>
	#... In every line, you can list one of your server. Note that there is no need to use any comma.
	)

```

7. Enjoy

## Contribution

Thanks for your issue, code and anything can help this repo.

## Liscence

MIT
