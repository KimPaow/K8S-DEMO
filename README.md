Create namespace for this demo:
`kubectl create ns k8sdemo`

List the pods in the namespace:
`kubectl get pods -n k8sdemo`
`kubectl get pods -n k8sdemo -o wide`

List the services in the namespace:
`kubectl get svc -n k8sdemo -o wide`

Apply the components:
`kubectl apply -n k8sdemo -f mongo-config.yaml`
`kubectl apply -n k8sdemo -f mongo-secret.yaml`
`kubectl apply -n k8sdemo -f mongo.yaml`
`kubectl apply -n k8sdemo -f webapp.yaml`

Get the Minikube ip:
`minikube ip`

Get the external ip and port of the webapp service:
`kubectl get svc -n k8sdemo -o wide`
