    {
      "kind": "main",
      "tag": "com-sap-sac-sample-echarts-sankeyyg",
      "url": "/main.js",
      "integrity": "sha256-HAHlBWe9J7FN0Zr5lPbBAkNpepQN3v4XXtmHgE2JOdY=",
      "ignoreIntegrity": false
    },
    {
      "kind": "styling",
      "tag": "com-sap-sac-sample-echarts-sankeyyg-styling",
      "url": "/sankeyChartStyling.js",
      "integrity": "sha256-AR0uDO+9h8nu9EyJotSinZ2APDWD5Ja2JmdFcZCH1Xo=",
      "ignoreIntegrity": false
    }
Uncaught (in promise) Error: [FailedAction - Action: dataAnalyzer.ui.setOpenDataAnalyzerEnabled@[{"app":"MAIN_APPLICATION"},{"story":"storyID"},{"table2":"96501675-2210-4920-8440-133451176415"},{"dataAnalyzer":"DataAnalyzerStoreEntityInstanceId"}] - Error: Store.InstanceNotFound/Can not execute action "dataAnalyzer.ui.setOpenDataAnalyzerEnabled" against instance [{"app":"MAIN_APPLICATION"},{"story":"storyID"},{"table2":"96501675-2210-4920-8440-133451176415"},{"dataAnalyzer":"DataAnalyzerStoreEntityInstanceId"}] which doesn't exist.]
    at new t (145.main.0035b23525bc4d9923fc.js:4:355)
    at t (145.main.0035b23525bc4d9923fc.js:5:46259)
    at F (145.main.0035b23525bc4d9923fc.js:5:45485)
    at n (145.main.0035b23525bc4d9923fc.js:5:46830)
    at 145.main.0035b23525bc4d9923fc.js:5:47026
    at 145.main.0035b23525bc4d9923fc.js:5:47328
    at d (145.main.0035b23525bc4d9923fc.js:1:8367)
    at 145.main.0035b23525bc4d9923fc.js:1:36334
    at 145.main.0035b23525bc4d9923fc.js:1:26210
    at Object.next (app.main.fee9a4f6ca9b5d7043f9.js:112:54387)
    at Object.next (app.main.fee9a4f6ca9b5d7043f9.js:112:53873)
    at n (145.main.0035b23525bc4d9923fc.js:6:74548)

    Failed to find a valid digest in the 'integrity' attribute for resource 'https://standard-chartered-q.ap11.hcs.cloud.sap/sap/fpa/services/rest/fpa/customWidgetComponent?widgetId=sdk_com_sap_sac_sample_echarts_sankeyyg&version=1&componentKind=styling' with computed SHA-256 integrity '47DEQpj8HBSa+/TImW+5JCeuQeRkm5NMpJWZG3hSuFU='. The resource has been blocked.
Failed to find a valid digest in the 'integrity' attribute for resource 'https://standard-chartered-q.ap11.hcs.cloud.sap/sap/fpa/services/rest/fpa/customWidgetComponent?widgetId=sdk_com_sap_sac_sample_echarts_sankeyyg&version=1&componentKind=main' with computed SHA-256 integrity '47DEQpj8HBSa+/TImW+5JCeuQeRkm5NMpJWZG3hSuFU='. The resource has been blocked.
app.chunk.1545.011fa…6b486c0f5af3d.js:21 
 Something went wrong. The system couldnt load the custom widget com.sap.sac.sample.echarts.sankeyyg_1.x (kind: styling). Please contact your system administrator or the owner of the custom widget.
