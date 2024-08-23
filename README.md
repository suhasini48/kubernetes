create cluster using ` eksctl create cluster -f cluster1.yml` <br />
create storageSlass  ` kubectl apply -f create_storage.yml ` <br />
create PVC(persistent volume Claim) ` kubectl apply -f claimstorage.yml ` <br />
deploy and create service(service for creating a standard end point to connect pvc on the fly ) for MonngoDB  ` kubectl apply -f mongodb_deploy.yml ` && ` kubectl apply -f monogo_service.yml ` <br />
deploy and create service for nodeWebApp ` kubectl apply -f nodeapp_deploy.yml ` &&  ` kubectl apply -f nodeapp_elb_service.yml ` <br />
