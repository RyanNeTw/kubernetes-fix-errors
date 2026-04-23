## Error 1

kubectl apply -R -f .

Error message : The Deployment "redis" is invalid: spec.template.spec.containers[0].volumeMounts[0].name: Not found: "redis-data"

redis/deployment.yaml => add spec/volumes

## Error 2

01/frontend/deployment.yaml => image: nginx:latest => Error d'orthographe

## Error 3

api/deployment.yaml => cpu: "100m"  => Diminuer le CPU a 0,1

## Error 4

api/deployment.yaml => port: 5000 => Erreur de port tourne en 80 au lieu de 5000

## Error 5

api/deployment.yaml =>   path: /health => paht : /

## Error 6

api/deployment.yaml => Pas de configmap => ajout de envFrom

## Error 7

api/service.yaml =>  targetPort: 5000 => Erreur de port tourne en 5001 au lieu de 5000

## Error 8

ingress/ingress.yaml =>  name: fronted => Error d'orthographe

## Error 9

01-frontend/service.yaml =>  app: frontend-app => Error de label