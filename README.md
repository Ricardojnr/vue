# C#
# Introduction 
TODO: Admin Panel is the back-end of internal report, this project is responsable to handle differents front-end as well to handle the security with the other projects.

# Getting Started
1.	Simply clone the project and the run it
2.	Each Team should create a controller that will handle their specific front-end.
3.  Each Team should have their own front-end Project so it can be included the CDN link in the file.
4.  The follow example shows how to implement a new front-end in the project

```JS
    var vueLink = https://reviewcomponentsdev.azureedge.net/reviewreport/vue.min.js? + 'token';
    var reviewReportComponentLink = https://reviewcomponentsdev.azureedge.net/reviewreport/vue.min.js?/reviewreport/reviewreportpanel.umd.js?" + 'Token';   
```

```HTML
    <script src="@vueLink"></script>
    <script src="@reviewReportComponentLink"></script>

    <body>

    <div id="app">
        <review-report-panel></review-report-panel>
    </div>

    <script>
        new Vue({
            components: {
                'review-report-panel': reviewreportpanel
            }
        }).$mount('#app')
    </script>

```
* review-report-panel is the specific name of the vue component that will be renderer
* Token is a security that each project should implement from the CDN
