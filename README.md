# companion-module-avstumpfl-pixera
See HELP.md and LICENSE

# *12/16/2023*: 
# Changes to action.js, Actions Created by Cody Luketic Created from October/November 2023


## Timeline

**1. timeline_transport_extended**
    - *Created 10/31/2023*
    - Adds functionality to have transport changes be toggled, and to change the transport of either a sinlge timeline. multiple inputed timelines, or a single timeline.

**2. timeline_scrubcurrenttime**
    - *Updated 10/31/2023*
    - Allows the ability to move through the timeline by a set amount of frames. Negative frames equals going backwards.

**3. timelines_zoomfactor**
    - *Created 10/27/2023*
    - Allows the ability to change the zoom level on a selected timeline.

**4. timeline_select**
    - *Created 10/27/2023*
    - Allows the ability to select a timeline.

**5. timeline_moverenderorder**
    - *Created 10/27/2023*
    - Allows the ablity to move a selected timeline up or down in the render order amoungst other timelines.

**6. timeline_create_layer**
    - *Created 10/27/2023*
    - Allows the ability to create a layer with the given name on a selected timeline.

**7. timeline_create_cue**
    - *Updated 10/31/2023*
    - Allows the ability to create a cue with the given name, operation, and values on a selected timeline.

**8. timeline_removecues**
    - *Created 10/27/2023*
    - Allows the ability to remove all cues on a selected timeline.

**9. timeline_reset**
    - *Created 10/27/2023*
    - Allows the abilty to reset a selected timeline.

**10. timeline_speedfactor**
    - *Created 10/27/2023*
    - Allows the ability to change the speed a selected timeline plays. The speed factor can be increased above 1.0 to run faster or decreased below 1.0 to run slower.


## Session

**11. session_project**
    - *Updated 10/30/2023*
    - Allows for control over projects. Able to Save, Save As, Load, and Close.

**12. session_livesystem**
    - *Created 10/31/2023*
    - Allows for control over livesystems from the Session API calls. Able to Start, Stop, and Restart the systems.

**13. session_setvideostreamactivestate**
    - *Created 10/30/2023*
    - Allows the ability to activate or deactivate the selected devices video stream active state.


## Livesystem

**14. livesystem_engine**
    - *Created 10/27/2023*
    - Allows for control over livesystems from the Livesystem API calls. Able to Start, Close, Restart, Reset, and Wake Up the systems.
    - Can choose to do a single system, all systems, or all systems except the local system.

**15. livesystem_exportMappings**
    - *Created 10/30/2023*
    - Allows the ability to export the mappings on a livesystem to a given path.

**16. livesystem_setaudiomaster_volume**
    - *Updated 10/31/2023*
    - Allows the ability to set the volume on a livesystem's master channels to a given value.

**17. livesystem_setaudiomaster_mute**
    - *Updated 10/31/2023*
    - Allows the ability to mute the volume on a livesystem's master channel either manually or with a toggle.

**18. livesystem_setaudiotimecodeinput**
    - *Updated 10/31/2023*
    - Allows the ability to change the timecode input state on a livesystem's master channel.


## Output

**19. output_status**
    - *Created 11/7/2023*
    - Allows for control over an output. Able to Activate, Identify, Make Output an Aggregate, and Set Aggregate Dimensions.
    - Can choose to manually change some of these settings or set them to be toggled.

**20. output_assignment**
    - *Created 11/7/2023*
    - Allows the ability to assign an output to a projector.
    - ***NOTE*** The assignment for Screens was not working and so that code is commented out. Will need to revisit.


## Resource

**21. resource_system**
    - *Created 11/8/2023*
    - Allows for control over a resource's system assets. Able to Remove, Remove Including Assets, Delete Files on Systems, Delete Asset From Live System, Replace, Refresh, Reset Distribution Targets, Change Distribution Targets, and Distribute.
    - ***NOTE*** Did not implement the ability to move the resource to a Transcoding Folder due to odd issues implementing a list of these folders. Will need to revisit.

**22. resource_settings_general**
    - *Created 11/8/2023*
    - Allows for control over a resource's settings. Able to Set Name, Set Current Version, and Set DMX Id.

**23. resource_settings_textweb**
    - *Created 11/8/2023*
    - Allows for control over a Text and Web resource's settings. Able to Set Text, Set Font with Name, Set Horizontal Alignment, Set Vertical Alignment, Set Line Height, and Set Url

**24. resource_settings_color**
    - *Created 11/8/2023*
    - Allows for control over a Color resource's settings. Able to Set Use Gradient and Set Color at Index.
    - Can choose to manually use the gradient or set it to be toggled.

**25. resource_multiresource**
    - *Created 11/9/2023*
    - Allows for control over a Multiresource's settings. Able to Add Multiresource Item, Remove Multiresource Item by Index, Replace Multiresource Item by Index, Set Multiresource Resolution, Set Multiresource Item Size by Index, Set Multiresource Item Position by Index.

**26. resource_folder_settings**
    - *Updated 11/14/2023*
    - Allows for control over a folder's settings. Able to Set Name, Set DMX Id, Change Distribution Targets, and Reset Distribution Targets.

**27. resource_folder_content**
    - *Created 11/14/2023*
    - Allows for control over a folder's contents. Able to Create Folders From Path, Remove This, Remove This Including Assets, Refresh Resources, Remove All Contents, Remove All Contents Inclding Assets, Delete All Contents Assets From Livesystem.
    - ***NOTE*** Resource Id was not implemented due to the command not working correctly. Will need to revisit.

***NOTE***: resource_folder_transcode is not implemented due to some issue with getting the commands to work. Will need to revisit.


## Screen

**28. screen_transform**
    - *Created 11/3/2023*
    - Allows for control over a screen's transformation. Able to set the Position, Rotation, Scale, Position and Rotation, Position and Rotation and Scale.

**29. screen_perspective_transform**
    - *Created 11/6/2023*
    - Allows for control over a perspective's transformation. Able to set the Position, Position with Look at, Rotation, and can Snap Sorners to Screen.

**30. screen_camera_transform**
    - *Created 11/6/2023*
    - Allows for control over a camera's transformation. Able to set the Position, Position with Look at, Rotation.

**31. screen_studiocamera_transform**
    - *Created 11/6/2023*
    - Allows for control over a studio camera's transformation. Able to set the Position, Rotation, and Transformation.
    - ***NOTE*** Transformation and Lens Properties and Transformation and Lens Properties Extended were not implimented due to some issue with getting the cammands to work. Will need to revisit.

**32. screen_studiocamera_tracking**
    - *Created 11/6/2023*
    - Allows for the control over a studio camera's tracking data. Able to Pause Tracking Input, Use Position Properties From Tracking, and Use Rotation Properties From Tracking.
    - Can choose to manually change some of these settings or set them to be toggled.
 
**33. projector_transform**
    - *Created 11/6/2023*
    - Allows for control over a projector's transformation. Able to set the Position, and the Rotation.

**34. projector_blackout**
    - *Created 11/6/2023*
    - Allows the ability to blackout a projector.


# Changes to Pixera.js, Code Added by Cody Luketic Created from October/November 2023

## Init

**1. initLivesystems**
    - Will init the self.CHOICES_LIVESYSTEMNAME array.

**2. initOutputs**
    - Will init the self.CHOICES_OUTPUTNAME array.

**3. initStudioCameras**
    - Will init the self.CHOICES_STUDIOCAMERANAME array.

**4. initProjectors**
    - Will init the self.CHOICES_PROJECTORNAME array.

**5. initResources**
    - Will init the self.CHOICES_RESOURCENAME array.

**6. initResourceFolders**
    - Will init the self.CHOICES_RESOURCEFOLDERNAME array.


## Variables

**7. self.CHOICES_LIVESYSTEMNAME, self.CHOICES_LIVESYSTEMHANDLE**
    - two arrays used to hold the names and handles of all Live Systems in the connected Pixera project.

**8. self.CHOICES_OUTPUTNAME, self.CHOICES_OUTPUTHANDLE**
    - two arrays used to hold the names and handles of all Outputs in the connected Pixera project.

**9. self.CHOICES_STUDIOCAMERANAME, self.CHOICES_STUDIOCAMERAHANDLE**
    - two arrays used to hold the names and handles of all Studio Cameras in the connected Pixera project.

**10. self.CHOICES_PROJECTORNAME, self.CHOICES_PROJECTORHANDLE**
    - two arrays used to hold the names and handles of all Projectors in the connected Pixera project.

**11. self.CHOICES_RESOURCENAME, self.CHOICES_RESOURCEHANDLE**
    - two arrays used to hold the names and handles of all Resources in the connected Pixera project.

**8. self.CHOICES_RESOURCEFOLDERNAME, self.CHOICES_RESOURCEFOLDERHANDLE**
    - two arrays used to hold the names and handles of all Resource Folders in the connected Pixera project.

**9. self.INDEX_LIVESYSTEM**
    - An int which keeps track of the index to match the current Live System's handle with its name.

**10. self.INDEX_STUDIOCAMERA**
    - An int which keeps track of the index to match the current Studio Camera's handle with its name.

**11. self.INDEX_OUTPUT**
    - An int which keeps track of the index to match the current Output's handle with its name.

**12. self.INDEX_RESOURCE**
    - An int which keeps track of the index to match the current Resource's handle with its name.

**13. self.INDEX_RESOURCEFOLDER**
    - An int which keeps track of the index to match the current Resource Folder's handle with its name.


## Cases

**14. case 15: //Pixera.LiveSystems.getLiveSystems**
    - This case will get and store all Live Systems in the current Pixera connection into self.CHOICES_LIVESYSTEMNAME.

**15. case 16: //Pixera.LiveSystems.getName**
    - This case will get the name of a given Live System to store with the corresponding ID in self.CHOICES_LIVESYSTEMNAME.

**16. case 17: //Pixera.Screens.getStudioCameras**
    - This case will get and store all Studio Cameras in the current Pixera connection into self.CHOICES_STUDIOCAMERANAME.

**17. case 18: //Pixera.Screens.StudioCamera.getName**
    - This case will get the name of a given Studio Camera to store with the corresponding ID in self.CHOICES_STUDIOCAMERANAME.

**18. case 19: //Pixera.Projectors.getProjectors**
    - This case will get and store all Projectors in the current Pixera connection into self.CHOICES_PROJECTORNAME.

**19. case 20: //Pixera.Projectors.getName**
    - This case will get the name of a given Projector to store with the corresponding ID in self.CHOICES_PROJECTORNAME.

**20. case 21: //Pixera.LiveSystems.getLiveSystems**
    - This case will get all Live Systems in the current Pixera connection to look at their Enabled Outputs.

**21. case 22: //Pixera.LiveSystems.LiveSystem.getEnabledOutputs**
    - This case will get and store all Enabled Outputs of the selected Live System in the current Pixera connection into self.CHOICES_OUTPUTNAME.

**22. case 23: //Pixera.LiveSystems.Output.getName**
    - This case will get the name of a given Output to store with the corresponding ID in self.CHOICES_OUTPUTNAME.

**23. case 24: //Pixera.LiveSystems.LiveSystem.getAudioMasterMute**
    - This case will set the Audio Master Mute state on a Live System by toggling it back and forth.

**24. case 25: //Pixera.LiveSystems.Output.getActive**
    - This case will set the Activate state on an Output by toggling it back and forth.

**25. case 26: //Pixera.LiveSystems.Output.getIdentify**
    - This case will set the Identify state on an Output by toggling it back and forth.

**26. case 27: //Pixera.LiveSystems.Output.getIsOutputAggregate**
    - This case will set the Is Output Aggregate state on an Output by toggling it back and forth.

**27. case 28: //Pixera.Screens.StudioCamera.getTrackingInputPause**
    - This case will set the Tracking Input Pause state on an Output by toggling it back and forth.

**28. case 29: //Pixera.Screens.StudioCamera.getUsePositionPropertiesFromTracking**
    - This case will set the Use Position Properties From Tracking state on an Output by toggling it back and forth.

**29. case 30: //Pixera.Screens.StudioCamera.getUseRotationPropertiesFromTracking**
    - This case will set the Use Rotation Properties From Tracking state on an Output by toggling it back and forth.

**30. case 31: //Pixera.Projectors.Projector.getBlackout**
    - This case will set the Blackout state on a Projector by toggling it back and forth.

**31. case 32: //Pixera.Timelines.Timeline.createLayer**
    - This case will set the name on a layer using the given string.

**32. case 33: //Pixera.Timelines.Timeline.cueHandle -> Pixera.Timelines.Cue.blendToThis**
    - This case will blend to the selected cue over the selected time.

**33. case 34: //Pixera.Timelines.Timeline.getCurrentTime**
    - This case will blend to the selected cue over the selected time.

**34. case 35: //Pixera.Resources.getResources**
    - This case will get and store all Resources in the current Pixera connection into self.CHOICES_RESOURCENAME.

**35. case 36: //Pixera.Resources.Resource.getName**
    - This case will get the name of a given Resource to store with the corresponding ID in self.CHOICES_RESOURCENAME.

**36. case 37: //Pixera.Projectors.Projector.getUseGradient**
    - This case will set the useGradient state on a Resource by toggling it back and forth.

**37. case 46: //Pixera.Timelines.Layer.getIsLayerMuted, case 47: //Pixera.Timelines.Layer.getIsAudioMuted**
    - These cases will toggle the mute on a layer's opacity or audio, depending on which case is selected.

**38. case 48: //Pixera.Resources.getResources**
    - This case will get the Media folder in the current Pixera connection.

**39. case 49: //Pixera.Resources.ResourceFolder.getResources**
    - This case will get and store all Resource Folders in the Media folder the current Pixera connection into self.CHOICES_RESOURCEFOLDERNAME.

**40. case 50: //Pixera.Resources.ResourceFolder.getName**
    - This case will get the name of a given Resource to store with the corresponding ID in self.CHOICES_RESOURCEFOLDERNAME.