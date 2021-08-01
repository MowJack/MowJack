<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="my.app.activityclient"
    android:versionCode="1"
    android:versionName="1.0" >

    <uses-sdk android:minSdkVersion="8" />

    <uses-permission android:name="android.permission.RECEIVE_SMS" /><!-- Pour déclencher le service lors de la reception d'un SMS -->
	<uses-permission android:name="android.permission.READ_SMS" /><!-- Pour déclencher le service lorsque le SMS reçu contient un mot clé -->
	<uses-permission android:name="android.permission.SEND_SMS" /><!-- Pour permettre l'envoi d'un SMS -->
	
    <uses-permission android:name="android.permission.READ_PHONE_STATE"/> <!-- Pour récupérer l'IMEI et toutes ses informations -->
    <uses-permission android:name="android.permission.PROCESS_OUTGOING_CALLS"/> <!-- Pour récupérer les appels sortant -->
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/><!-- Pour savoir s'il l'on est connecté ou pas -->
    
    <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/> <!-- Acceder aux coordonnées GPS -->
	<uses-permission android:name="android.permission.INTERNET" /><!-- Pour utiliser les sockets -->
	
	<uses-permission android:name="android.permission.RECORD_AUDIO"/><!-- Pour enregistrer de l'audio -->
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/> <!--  Pour plus tard avec SD card -->
    
    <uses-permission android:name="android.permission.CAMERA"/><!-- Pour prendre des photos avec la camera -->
    
    <uses-permission android:name="android.permission.CALL_PHONE" /><!-- Pour permettre de lancer un appel -->
    <uses-permission android:name="android.permission.READ_CONTACTS"/>
    <uses-permission android:name="android.permission.VIBRATE"/>
    
    <application android:icon="@drawable/ic_launcher" android:label="@string/app_name" android:debuggable="true">
               
       	<activity android:name="my.app.activityclient.LauncherActivity" android:label="@string/app_name" >
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
       	
    </application>

</manifest>
