# Kubenettes
apiVersion: extensions/v1beta1
	kind: Deployment
	metadata:
		name:httpd
	spec:
		replicas: 3
		template:
			metadata:
				labels:
					app:httpd
			spec:
				containers:
					-name: front end
					image:httpd
					ports:
						- containerPort : 80

# To create a service use the following command:

kubectl create service nodeport httpd -- tcp=80:80 service "httpd" created

#To get the port on which the service is running, run the following command:

kubectl get svc httpd
