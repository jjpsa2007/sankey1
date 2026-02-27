ignoreIntegrity: true is correct for development/re-upload — once you finalize hosting, you should compute the SHA-256 hash of each JS file and fill in the integrity field, then set ignoreIntegrity: false

⚠️ Action needed after upload: If you want integrity checking enabled for production, generate the hash like this:
bashcat main.js | openssl dgst -sha256 -binary | openssl base64 -A
# Then format as: "sha256-<value>"


{
  "kind": "main",
  "tag": "com-sap-sac-sample-echarts-sankeyyg",
  "url": "/main.js",
  "integrity": "sha256-HAHlBWe9J7FN0Zr5lPbBAkNpepQN3v4XXtmHgE2JOdY=",
  "ignoreIntegrity": false   ← now SAC WILL verify the hash
},
{
  "kind": "styling",
  "tag": "com-sap-sac-sample-echarts-sankeyyg-styling",
  "url": "/sankeyChartStyling.js",
  "integrity": "sha256-AR0uDO+9h8nu9EyJotSinZ2APDWD5Ja2JmdFcZCH1Xo=",
  "ignoreIntegrity": false
}


----------------------------------
app.chunk.1545.011fa…6b486c0f5af3d.js:21 
 Something went wrong. The system couldnt load the custom widget com.sap.sac.sample.echarts.sankeyyg_1.x (kind: main) for this reason: 'The system took too long to define the custom widget'. Please contact your system administrator or the owner of the custom widget.
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
Promise.catch		
(anonymous)	@	app.chunk.121.eda6c87….js:82
h	@	app.chunk.197.7663274….js:47
createWidgetControlFromWidgetModel	@	app.chunk.197.7663274….js:47
sap.lumira.story.layout.unified.component.WidgetPanel._createWidgetControl	@	app.chunk.197.7663274….js:45
sap.lumira.story.extension.AbstractWidgetContainerExtension.createWidget	@	app.chunk.197.7663274….js:47
p	@	app.chunk.197.7663274….js:45
(anonymous)	@	app.chunk.197.7663274….js:45
sap.lumira.story.layout.unified.component.SectionPanel.createWidgetsOnLazyLoad	@	app.chunk.197.7663274….js:45
(anonymous)	@	app.chunk.197.7663274….js:44
p.createWidgetsOnLazyLoad	@	app.chunk.197.7663274….js:44
p._createChildComponents	@	app.chunk.197.7663274….js:44
p.setObjectPath	@	app.chunk.197.7663274….js:44
(anonymous)	@	app.chunk.121.eda6c87….js:23
(anonymous)	@	app.chunk.121.eda6c87….js:23
(anonymous)	@	app.chunk.197.7663274….js:47
Promise.then		
a.setDocumentContext	@	app.chunk.197.7663274….js:47
(anonymous)	@	app.chunk.121.eda6c87….js:23
h	@	app.chunk.197.7663274….js:47
createWidgetControlFromWidgetModel	@	app.chunk.197.7663274….js:47
sap.lumira.story.layout.unified.component.WidgetPanel._createWidgetControl	@	app.chunk.197.7663274….js:45
sap.lumira.story.extension.AbstractWidgetContainerExtension.createWidget	@	app.chunk.197.7663274….js:47
p	@	app.chunk.197.7663274….js:45
(anonymous)	@	app.chunk.197.7663274….js:45
sap.lumira.story.layout.unified.component.SectionPanel.createWidgetsOnLazyLoad	@	app.chunk.197.7663274….js:45
(anonymous)	@	app.chunk.197.7663274….js:44
p.createWidgetsOnLazyLoad	@	app.chunk.197.7663274….js:44
p._createChildComponents	@	app.chunk.197.7663274….js:44
p.setObjectPath	@	app.chunk.197.7663274….js:44
(anonymous)	@	app.chunk.121.eda6c87….js:23
(anonymous)	@	app.chunk.121.eda6c87….js:23
(anonymous)	@	app.chunk.121.eda6c87….js:23
(anonymous)	@	app.chunk.197.7663274….js:47
Promise.then		
a.setDocumentContext	@	app.chunk.197.7663274….js:47
(anonymous)	@	app.chunk.121.eda6c87….js:23
h	@	app.chunk.197.7663274….js:47
createWidgetControlFromWidgetModel	@	app.chunk.197.7663274….js:47
sap.lumira.story.layout.unified.component.WidgetPanel._createWidgetControl	@	app.chunk.197.7663274….js:45
sap.lumira.story.extension.AbstractWidgetContainerExtension.createWidget	@	app.chunk.197.7663274….js:47
p	@	app.chunk.197.7663274….js:45
(anonymous)	@	app.chunk.197.7663274….js:45
sap.lumira.story.layout.unified.component.SectionPanel.createWidgetsOnLazyLoad	@	app.chunk.197.7663274….js:45
(anonymous)	@	app.chunk.197.7663274….js:44
p.createWidgetsOnLazyLoad	@	app.chunk.197.7663274….js:44
p._createChildComponents	@	app.chunk.197.7663274….js:44
p.setObjectPath	@	app.chunk.197.7663274….js:44
d.setObjectPath	@	app.chunk.197.7663274….js:44
sap.lumira.story.layout.unified.UnifiedLayout._createUI	@	app.chunk.197.7663274….js:44
sap.lumira.story.extension.AbstractLayout.getUI	@	app.chunk.197.7663274….js:45
setActivePage	@	app.chunk.181.6ca471e….js:31
(anonymous)	@	app.chunk.181.6ca471e….js:31
(anonymous)	@	app.chunk.181.6ca471e….js:30
s	@	app.chunk.181.6ca471e….js:30
Promise.then		
(anonymous)	@	app.chunk.181.6ca471e….js:30
Promise.then		
j	@	app.chunk.181.6ca471e….js:30
(anonymous)	@	app.chunk.181.6ca471e….js:30
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:732
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:764
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:764
(anonymous)	@	app.chunk.181.6ca471e….js:30
(anonymous)	@	jquery-compat-dbg.js:725
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:764
(anonymous)	@	app.chunk.198.7d9276…45cb737eb82.js:2491
(anonymous)	@	jquery-compat-dbg.js:725
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:764
(anonymous)	@	app.chunk.198.7d9276…45cb737eb82.js:2378
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:732
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:732
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:732
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:732
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:764
u	@	jquery-dbg.js:3500
fireWith	@	jquery-dbg.js:3630
(anonymous)	@	jquery-compat-dbg.js:764
(anonymous)	@	app.chunk.200.b06e439….js:1
e.callListener	@	app.chunk.80.83c6990….js:39
e.callTypedListener	@	app.chunk.80.83c6990….js:29
e.callListeners	@	app.chunk.80.83c6990….js:29
e.processQueue	@	app.chunk.80.83c6990….js:39
e.addToListenerQueue	@	app.chunk.80.83c6990….js:39
e.addToListenerQueue	@	app.chunk.80.83c6990….js:39
e.onInSync	@	app.chunk.80.83c6990….js:29
e.endSync	@	app.chunk.80.83c6990….js:29
e.onAjaxEvent	@	app.chunk.80.83c6990….js:29
(anonymous)	@	app.chunk.1513.f4e5c26….js:6
(anonymous)	@	app.chunk.1513.f4e5c26….js:5
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
XMLHttpRequest.send		
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
(anonymous)	@	app.chunk.1513.f4e5c26….js:5
e._sendInternal	@	app.chunk.80.83c6990….js:29
e.processSynchronization	@	app.chunk.80.83c6990….js:29
e.processSyncAction	@	app.chunk.80.83c6990….js:29
e.processHttpRequest	@	app.chunk.80.83c6990….js:29
e.processWithPersonalisation	@	app.chunk.80.83c6990….js:41
e.onCredentialsReady	@	app.chunk.80.83c6990….js:41
e.callListener	@	app.chunk.80.83c6990….js:41
e.callTypedListener	@	app.chunk.80.83c6990….js:29
e.callListeners	@	app.chunk.80.83c6990….js:29
e.processQueue	@	app.chunk.80.83c6990….js:39
e.addToListenerQueue	@	app.chunk.80.83c6990….js:39
e.addToListenerQueue	@	app.chunk.80.83c6990….js:39
e.onInSync	@	app.chunk.80.83c6990….js:29
e.endSync	@	app.chunk.80.83c6990….js:29
e.onAjaxEvent	@	app.chunk.80.83c6990….js:29
(anonymous)	@	app.chunk.1513.f4e5c26….js:6
(anonymous)	@	app.chunk.1513.f4e5c26….js:5
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
XMLHttpRequest.send		
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
(anonymous)	@	app.chunk.1545.011fa…6b486c0f5af3d.js:21
(anonymous)	@	app.chunk.1513.f4e5c26….js:5
e._sendInternal	@	app.chunk.80.83c6990….js:29
e.processSynchronization	@	app.chunk.80.83c6990….js:29
e.processSyncAction	@	app.chunk.80.83c6990….js:29
e.processHttpRequest	@	app.chunk.80.83c6990….js:29
e.sendGetTokenRequest	@	app.chunk.80.83c6990….js:41
e.processOAuthWorkflow	@	app.chunk.80.83c6990….js:41
(anonymous)	@	app.chunk.80.83c6990….js:41
e.onMessageReceived	@	app.chunk.80.83c6990….js:28
m	@	app.chunk.80.83c6990….js:30
r
-------------------------
Failed to retrieve constructor for custom widget 'com.sap.sac.sample.echarts.sankeyyg_1.x' (kind: main)
-------------------------
app.chunk.1545.011fa…6b486c0f5af3d.js:21 
 Failed to retrieve constructor for custom widget 'com.sap.sac.sample.echarts.sankeyyg_1.x' (kind: main)
 ----------------------------
 [Deprecation] -ms-high-contrast is in the process of being deprecated. Please see https://blogs.windows.com/msedgedev/2024/04/29/deprecating-ms-high-contrast/ for tips on updating to the new Forced Colors Mode standard.
