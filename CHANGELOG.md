# eppz.Cloud

* 0.5.0

	+ Added value types
		+ `EPPZ_Cloud_StringForKey` / `EPPZ_Cloud_SetStringForKey`
		+ `EPPZ_Cloud_FloatForKey` / `EPPZ_Cloud_SetFloatForKey`
		+ `EPPZ_Cloud_IntForKey` / `EPPZ_Cloud_SetIntForKey`
		+ `EPPZ_Cloud_BoolForKey` / `EPPZ_Cloud_SetBoolForKey`
	+ iOS Sandbox app implemented
		+ Hooked up UI outlets / actions
		+ Added keys with corresponding actions (blocks)
		+ Implemented per value conflict resolution strategies

* 0.4.2

	+ Built iOS Sandbox app test UI
		+ Explored auto layout constraints / stack views

* 0.4.0

	+ Implemented Unity plugin architecture
		+ `Plugin.Cloud` common plugin base class
		+ Individual platform implementations
			+ `Plugin.Cloud_iOS`
			+ `Plugin.Cloud_Android`
			+ `Plugin.Cloud_Editor`
		+ Key-value update models (key-value pair model hooks)
			+ Events can be invoked on remote updates
		+ `Cloud : MonoBehaviour` class for scene use
			+ Native plugins sends message(s) to this `GameObject`
			+ Key-value update models can be hooked up here
			+ Encapsulates various platform implementations
		+ `Plugin.Cloud_iOS` DLL imports implemented / hooked up
			+ Copy Files Phase for `eppz! Cloud.a` have setup

* 0.0.2

	+ Added `iOS~` native plugin project 
		+ Uses Key-Value store
		+ Can be tested directly in Xcode sandbox iOS project (actually on device)
		+ `NSNotification.userInfo` sent directly to Unity (via JSON)

* 0.0.1

	+ Initial commit