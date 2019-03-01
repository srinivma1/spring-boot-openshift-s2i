# spring-boot-openshift-s2i

Use oc create -f spring-boot-template.yml to create the Openshift objects.

For creating configmaps, use following command:

 oc create configmap <config file name> --from-file=src/main/resources/application.properties
  
This should match with config file name in the templates i.e. this:

          configMap:
            name:  route-2a-config 
