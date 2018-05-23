# README

This bundle plugin provides a portlet that can be used to display google analytic data within dotCMS' administrative.


## How to build this example

To install all you need to do is build the JAR. to do this run
`./gradlew jar`
This will build a jar in the build/libs directory

* To install this bundle:
    Copy the bundle jar file inside the Felix OSGI container (dotCMS/felix/load).
            OR
    Upload the bundle jar file using the dotCMS UI (CMS Admin->Dynamic Plugins->Upload Plugin).

* To uninstall this bundle:
    Remove the bundle jar file from the Felix OSGI container (dotCMS/felix/load).
            OR
    Undeploy the bundle using the dotCMS UI (CMS Admin->Dynamic Plugins->Undeploy).

### Multi language support

The creation of the Portlets will generate the following language key and it as the title for the Portlets:
`javax.portlet.title.EXT_GA_DASHBOARD`


In order to add multilanguage values for this key:
*CMS Admin* -> *Language Variables* -> *Edit Default Language Variables* -> Add the values for the above key
  	
