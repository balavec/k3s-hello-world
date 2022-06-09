# k3s-hello-world

Prepare k3s on an AWS EC2 instance for example:

    sudo apt update
    sudo apt upgrade
    sudo apt install -y curl
    sudo curl -sfL https://get.k3s.io | sh -

## Example k3s hello world deployment

Source: https://www.jeffgeerling.com/blog/2022/quick-hello-world-http-deployment-testing-k3s-and-traefik

Run:

    sudo k3s kubectl create configmap hello-world --from-file index.html
    sudo k3s kubectl apply -f hello-world.yml
