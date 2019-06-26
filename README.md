# Kubenettes

# To create a service use the following command:
kubectl create service nodeport httpd -- tcp=80:80 service "httpd" created

# To get the port on which the service is running, run the following command:

kubectl get svc httpd

# Access Dash board
kubectl proxy starting to serve on 127.0.0.1:8001
