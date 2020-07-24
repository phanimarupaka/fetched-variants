Anthos CI/CD clusters layer
==================================================

# NAME

  clusters

# SYNOPSIS

To apply the package:

    kubectl apply -R -f clusters/

To edit the package:

    kpt cfg list-setters clusters/
    
         NAME           VALUE        SET BY            DESCRIPTION             COUNT   REQUIRED  
      environment   ENV                       Environment of the cluster       21      Yes       
      namespace     YOUR_NAMESPACE            Namespace of Config Connector    3       Yes       
                                              resources                                          
      project-id    YOUR_PROJECT              Project ID where the cluster     1       Yes       
                                              will run                                           
      region        REGION                    Region of the cluster            21      Yes       

    
    
    kpt cfg set clusters/ SETTER VALUE

# Description

You can apply this across multiple environments and regions by setting appropriate setters

# SEE ALSO

[0_foundation](../0_foundation/) package