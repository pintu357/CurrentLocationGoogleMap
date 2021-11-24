Make Change in Manifest File :

//Add Permissions
<uses-permission android:name="android.permission.INTERNET"/>
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
    
 Add Meta-Data( Here value is GoogleMap generated Token) 
<meta-data
            android:name="com.google.android.geo.API_KEY"
            android:value="AIzaSyA7RuwEE1lC_L_n_9aBlPbfcWds6RXPkD4"/>
            
            
  
  
  
  
  //Add Dependency in gradle Module :app
	  implementation 'com.google.android.gms:play-services-maps:18.0.0'
    implementation 'com.google.android.gms:play-services-location:18.0.0'

    implementation 'com.karumi:dexter:6.2.3'( It is for taking runtime Permissions)
		<activity-------------------------------------------->
		
		
		
		// Make MainActivity Layout like this(i.e RelativeLayout & fragment)
		<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <fragment
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:id="@+id/google_map"
        android:name="com.google.android.gms.maps.SupportMapFragment"/>

</RelativeLayout>


// Rest of the code write in MainActivity.java class

	
	
	
	
