# facet_config_searchportlet_hook
This hook was developed for changing the default facet configuration value that is used by the Velocity variable $theme.search().   Since the search portlet is embbeded in the theme through the Velocity variable $theme.search(), there is no way to change the facets search configs, except by hooking.

This hook overwrites the following files in the /portlet/search/ folder: 
 - search.jsp (change the facet configuration)
 - configuration.jsp (add a warning message in the configuration modal)
 - opensearch.jsp (disable opensearch features completely due to technical conflicts)
 
 Note: While this hook is active in the portal any additional configuration made in the configuration page will have effect. If you want to set up a custom configuration using the configuration page you must disable this hook on your portal.
