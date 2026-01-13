# BuzzIntell Trust-Zero — Public Overview

BuzzIntell Trust-Zero is a safety-first architecture
designed to reduce abuse in email and calendar systems.

It works by documenting how trust artifacts should be
handled safely — without surveillance or intrusion.

---

## What This Is

- A defensive design framework
- A governance and policy system
- A non-interactive safety model

---

## What This Is Not

- Not spyware
- Not monitoring software
- Not an email scanner
- Not a tracking system

---

## Why It Exists

Email and calendars are trusted by default.
That trust is frequently abused.

BuzzIntell Trust-Zero shows how to neutralize that risk
without reading messages or watching users.

---

## Core Principles

- Trust-Zero
- Privacy-by-design
- Non-interference
- Governance-first

---

## Transparency

This repository contains documentation only.
There is no running system.This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>This XML file does not appear to have any style information associated with it. The document tree is shown below.
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="8081203" android:versionName="v1.0.6" android:compileSdkVersion="36" android:compileSdkVersionCodename="16" android:requiredSplitTypes="base__abi,base__density" android:splitTypes="" package="com.taxwell.mobilized" platformBuildVersionCode="36" platformBuildVersionName="16">
<uses-sdk android:minSdkVersion="24" android:targetSdkVersion="36"/>
<uses-permission android:name="android.permission.USE_BIOMETRIC"/>
<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
<uses-permission android:name="android.permission.CAMERA"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-feature android:name="android.hardware.camera" android:required="true"/>
<uses-feature android:name="android.hardware.camera.autofocus" android:required="false"/>
<uses-permission android:name="android.permission.INTERNET"/>
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE"/>
<uses-permission android:name="com.google.android.gms.permission.AD_ID"/>
<uses-permission android:name="android.permission.WAKE_LOCK"/>
<uses-permission android:name="android.permission.ACCESS_WIFI_STATE"/>
<queries>
<intent>
<action android:name="android.intent.action.GET_CONTENT"/>
<data android:mimeType="*/*"/>
</intent>
<intent>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https"/>
</intent>
<intent>
<action android:name="com.appsflyer.referrer.INSTALL_PROVIDER"/>
</intent>
<package android:name="com.facebook.katana"/>
<package android:name="com.instagram.android"/>
<package android:name="com.facebook.lite"/>
<package android:name="com.samsung.android.mapsagent"/>
</queries>
<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE"/>
<uses-permission android:name="android.permission.RECORD_AUDIO"/>
<uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION"/>
<uses-permission android:name="com.samsung.android.mapsagent.permission.READ_APP_INFO"/>
<uses-permission android:name="com.huawei.appmarket.service.commondata.permission.GET_COMMON_DATA"/>
<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID"/>
<permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION" android:protectionLevel="0x00000002"/>
<uses-permission android:name="com.taxwell.mobilized.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION"/>
<application android:label="TaxAct" android:icon="@7F0D0001" android:name="android.app.Application" android:allowBackup="true" android:extractNativeLibs="false" android:fullBackupContent="@7F120000" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:dataExtractionRules="@7F120001">
<activity android:theme="@7F1000A3" android:name="com.taxwell.mobilized.MainActivity" android:exported="true" android:launchMode="1" android:configChanges="0x40003FB4" android:windowSoftInputMode="0x00000010" android:hardwareAccelerated="true">
<meta-data android:name="io.flutter.embedding.android.NormalTheme" android:resource="@7F1000A4"/>
<intent-filter>
<action android:name="android.intent.action.MAIN"/>
<category android:name="android.intent.category.LAUNCHER"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="mfa.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="ppd.taxact.com" android:pathPrefix="/mobile"/>
<data android:scheme="https" android:host="taxact.com" android:pathPrefix="/mobile"/>
</intent-filter>
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="tst-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.tst/callback"/>
<data android:scheme="https" android:host="mfa-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.mfa/callback"/>
<data android:scheme="https" android:host="ppd-auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized.ppd/callback"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
<intent-filter>
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="taxact"/>
</intent-filter>
</activity>
<activity android:name="com.auth0.android.provider.RedirectActivity" android:exported="true">
<intent-filter android:autoVerify="true">
<action android:name="android.intent.action.VIEW"/>
<category android:name="android.intent.category.DEFAULT"/>
<category android:name="android.intent.category.BROWSABLE"/>
<data android:scheme="https" android:host="auth.taxact.com" android:pathPrefix="/android/com.taxwell.mobilized/callback"/>
</intent-filter>
</activity>
<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.fileprovider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120002"/>
</provider>
<meta-data android:name="flutterEmbedding" android:value="2"/>
<service android:name="androidx.credentials.playservices.CredentialProviderMetadataHolder" android:enabled="true" android:exported="false">
<meta-data android:name="androidx.credentials.CREDENTIAL_PROVIDER_KEY" android:value="androidx.credentials.playservices.CredentialProviderPlayServicesImpl"/>
</service>
<activity android:theme="@7F10012D" android:name="androidx.credentials.playservices.HiddenActivity" android:enabled="true" android:exported="false" android:configChanges="0x000005A0" android:fitsSystemWindows="true"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true"/>
<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" android:visibleToInstantApps="true"/>
<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.analytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.firebaseremoteconfig.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.crashlytics.FlutterFirebaseAppRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:io.flutter.plugins.firebase.core.FlutterFirebaseCoreRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.FirebaseRemoteConfigKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.FirebaseCrashlyticsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.crashlytics.CrashlyticsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.sessions.FirebaseSessionsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.installations.FirebaseInstallationsRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.FirebaseCommonKtxRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.firebase.datatransport.TransportRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="io.flutter.plugins.imagepicker.ImagePickerFileProvider" android:exported="false" android:authorities="com.taxwell.mobilized.flutter.image_provider" android:grantUriPermissions="true">
<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@7F120003"/>
</provider>
<service android:name="com.google.android.gms.metadata.ModuleDependencies" android:enabled="false" android:exported="false">
<intent-filter>
<action android:name="com.google.android.gms.metadata.MODULE_DEPENDENCIES"/>
</intent-filter>
<meta-data android:name="photopicker_activity:0:required" android:value=""/>
</service>
<activity android:theme="@android:01030007" android:name="io.flutter.plugins.urllauncher.WebViewActivity" android:exported="false"/>
<activity android:theme="@android:0103000A" android:name="com.google.mlkit.vision.documentscanner.internal.GmsDocumentScanningDelegateActivity" android:exported="false" android:screenOrientation="1"/>
<service android:name="com.google.mlkit.common.internal.MlKitComponentDiscoveryService" android:exported="false" android:directBootAware="true">
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.text.internal.TextRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.vision.common.internal.VisionCommonRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
<meta-data android:name="com.google.firebase.components:com.google.mlkit.common.internal.CommonComponentRegistrar" android:value="com.google.firebase.components.ComponentRegistrar"/>
</service>
<provider android:name="com.google.mlkit.common.internal.MlKitInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.mlkitinitprovider" android:initOrder="99"/>
<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false"/>
<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false"/>
<activity android:theme="@android:01030010" android:name="com.auth0.android.provider.AuthenticationActivity" android:exported="false" android:launchMode="2" android:configChanges="0x00000DB0"/>
<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.taxwell.mobilized.firebaseinitprovider" android:initOrder="100" android:directBootAware="true"/>
<provider android:name="androidx.startup.InitializationProvider" android:exported="false" android:authorities="com.taxwell.mobilized.androidx-startup">
<meta-data android:name="androidx.emoji2.text.EmojiCompatInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.lifecycle.ProcessLifecycleInitializer" android:value="androidx.startup"/>
<meta-data android:name="androidx.profileinstaller.ProfileInstallerInitializer" android:value="androidx.startup"/>
</provider>
<uses-library android:name="androidx.window.extensions" android:required="false"/>
<uses-library android:name="androidx.window.sidecar" android:required="false"/>
<uses-library android:name="android.ext.adservices" android:required="false"/>
<meta-data android:name="com.google.android.gms.version" android:value="@7F0A0004"/>
<receiver android:name="androidx.profileinstaller.ProfileInstallReceiver" android:permission="android.permission.DUMP" android:enabled="true" android:exported="true" android:directBootAware="false">
<intent-filter>
<action android:name="androidx.profileinstaller.action.INSTALL_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SKIP_FILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.SAVE_PROFILE"/>
</intent-filter>
<intent-filter>
<action android:name="androidx.profileinstaller.action.BENCHMARK_OPERATION"/>
</intent-filter>
</receiver>
<service android:name="com.google.android.datatransport.runtime.backends.TransportBackendDiscovery" android:exported="false">
<meta-data android:name="backend:com.google.android.datatransport.cct.CctBackendFactory" android:value="cct"/>
</service>
<service android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.JobInfoSchedulerService" android:permission="android.permission.BIND_JOB_SERVICE" android:exported="false"/>
<receiver android:name="com.google.android.datatransport.runtime.scheduling.jobscheduling.AlarmManagerSchedulerBroadcastReceiver" android:exported="false"/>
<activity android:theme="@7F10012E" android:name="com.google.android.play.core.common.PlayCoreDialogWrapperActivity" android:exported="false" android:stateNotNeeded="true"/>
<activity android:name="com.pairip.licensecheck.LicenseActivity" android:exported="false"/>
<provider android:name="com.pairip.licensecheck.LicenseContentProvider" android:exported="false" android:authorities="com.taxwell.mobilized.com.pairip.licensecheck.LicenseContentProvider"/>
<meta-data android:name="com.android.vending.splits.required" android:value="true"/>
<meta-data android:name="com.android.stamp.source" android:value="https://play.google.com/store"/>
<meta-data android:name="com.android.stamp.type" android:value="STAMP_TYPE_DISTRIBUTION_APK"/>
<meta-data android:name="com.android.vending.splits" android:resource="@7F120005"/>
<meta-data android:name="com.android.vending.derived.apk.id" android:value="3"/>
</application>
<uses-permission android:name="com.android.vending.CHECK_LICENSE"/>
</manifest>
