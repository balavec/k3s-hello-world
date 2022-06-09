# k3s-hello-world

Example k3s hello world deployment

Source: https://www.jeffgeerling.com/blog/2022/quick-hello-world-http-deployment-testing-k3s-and-traefik

Run:

    kubectl create configmap hello-world --from-file index.html
    kubectl apply -f hello-world.yml
