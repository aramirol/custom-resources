# docker.sock

To automate the docker.sock permissions follow these steps:

1. Download files:
   ```sh
   wget https://github.com/aramirol/custom-resources/blob/main/kubernetes/docker.sock/docker_sock_acl.sh
   wget https://github.com/aramirol/custom-resources/blob/main/kubernetes/docker.sock/docker_sock.service
   ```

2. Copy files and apply permissions:
   ```sh
   cp docker_sock_acl.sh <path_you_want>
   chmod 744 <path_you_want>/docker_sock_acl.sh
   cp docker_sock.service /etc/systemd/system/docker_sock.service
   ```

3. Reload and enable new service:
   ```sh
   sysmtectl daemon-reload
   systemctl enable docker_sock.service
   systemctl start docker_sock.service
   ```

After that, you can restart your server and check that the permissions have changed automatically.
