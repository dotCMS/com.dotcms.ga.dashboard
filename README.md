# README

This bundle plugin provides a portlet that can be used to display google analytic data within dotCMS' administrative.


## Prerequisites

1. Make sure you are using Google Analytics on your web property

2. You need to create a dashboard using https://datastudio.google.com.  Doing so will give you the embed code to use with the portlet view.vtl.  To get you started, you can clone this template which is filled with dummy data: https://datastudio.google.com/u/0/reporting/1cWJ9dg0BOU-fQ7I0OpTsAwR9UWy-V7hg/page/sBV

3. Replace the src="https://datastudio.google.com/embed/reporting/XXXXXXXXXXXXXXXXXX/page/xxx"  here https://github.com/dotCMS/com.dotcms.ga.dashboard/blob/master/src/main/resources/ext/view.vtl#L1  with the embed link to your new google dashboard.


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
  	
