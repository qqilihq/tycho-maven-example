Very short reduced example for this Stack Overflow question:

http://stackoverflow.com/questions/41213928/transitive-dependencies-not-resolved-with-maven-dependency-and-tycho-pomconsider

Our workflow is as follows:

1. `01_bundle_wrappers` creates bundle wrappers for non-OSGi dependencies
2. `02_update_site_for_dependencies` builds an update site with the Maven dependencies from previous step, this can later also be used in the Eclipse IDE
3. `03_actual_product` builds the actual Eclipse plugin
