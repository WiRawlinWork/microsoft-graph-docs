---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Windows10GeneralConfiguration
{
	OdataType = "#microsoft.graph.windows10GeneralConfiguration",
	Description = "Description value",
	DisplayName = "Display Name value",
	Version = 7,
	EnterpriseCloudPrintDiscoveryEndPoint = "Enterprise Cloud Print Discovery End Point value",
	EnterpriseCloudPrintOAuthAuthority = "Enterprise Cloud Print OAuth Authority value",
	EnterpriseCloudPrintOAuthClientIdentifier = "Enterprise Cloud Print OAuth Client Identifier value",
	EnterpriseCloudPrintResourceIdentifier = "Enterprise Cloud Print Resource Identifier value",
	EnterpriseCloudPrintDiscoveryMaxLimit = 5,
	EnterpriseCloudPrintMopriaDiscoveryResourceIdentifier = "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
	SearchBlockDiacritics = true,
	SearchDisableAutoLanguageDetection = true,
	SearchDisableIndexingEncryptedItems = true,
	SearchEnableRemoteQueries = true,
	SearchDisableIndexerBackoff = true,
	SearchDisableIndexingRemovableDrive = true,
	SearchEnableAutomaticIndexSizeManangement = true,
	DiagnosticsDataSubmissionMode = DiagnosticDataSubmissionMode.None,
	OneDriveDisableFileSync = true,
	SmartScreenEnableAppInstallControl = true,
	PersonalizationDesktopImageUrl = "https://example.com/personalizationDesktopImageUrl/",
	PersonalizationLockScreenImageUrl = "https://example.com/personalizationLockScreenImageUrl/",
	BluetoothAllowedServices = new List<string>
	{
		"Bluetooth Allowed Services value",
	},
	BluetoothBlockAdvertising = true,
	BluetoothBlockDiscoverableMode = true,
	BluetoothBlockPrePairing = true,
	EdgeBlockAutofill = true,
	EdgeBlocked = true,
	EdgeCookiePolicy = EdgeCookiePolicy.Allow,
	EdgeBlockDeveloperTools = true,
	EdgeBlockSendingDoNotTrackHeader = true,
	EdgeBlockExtensions = true,
	EdgeBlockInPrivateBrowsing = true,
	EdgeBlockJavaScript = true,
	EdgeBlockPasswordManager = true,
	EdgeBlockAddressBarDropdown = true,
	EdgeBlockCompatibilityList = true,
	EdgeClearBrowsingDataOnExit = true,
	EdgeAllowStartPagesModification = true,
	EdgeDisableFirstRunPage = true,
	EdgeBlockLiveTileDataCollection = true,
	EdgeSyncFavoritesWithInternetExplorer = true,
	CellularBlockDataWhenRoaming = true,
	CellularBlockVpn = true,
	CellularBlockVpnWhenRoaming = true,
	DefenderRequireRealTimeMonitoring = true,
	DefenderRequireBehaviorMonitoring = true,
	DefenderRequireNetworkInspectionSystem = true,
	DefenderScanDownloads = true,
	DefenderScanScriptsLoadedInInternetExplorer = true,
	DefenderBlockEndUserAccess = true,
	DefenderSignatureUpdateIntervalInHours = 6,
	DefenderMonitorFileActivity = DefenderMonitorFileActivity.Disable,
	DefenderDaysBeforeDeletingQuarantinedMalware = 12,
	DefenderScanMaxCpu = 2,
	DefenderScanArchiveFiles = true,
	DefenderScanIncomingMail = true,
	DefenderScanRemovableDrivesDuringFullScan = true,
	DefenderScanMappedNetworkDrivesDuringFullScan = true,
	DefenderScanNetworkFiles = true,
	DefenderRequireCloudProtection = true,
	DefenderCloudBlockLevel = DefenderCloudBlockLevelType.High,
	DefenderPromptForSampleSubmission = DefenderPromptForSampleSubmission.AlwaysPrompt,
	DefenderScheduledQuickScanTime = new Time(DateTime.Parse("11:58:49.3840000")),
	DefenderScanType = DefenderScanType.Disabled,
	DefenderSystemScanSchedule = WeeklySchedule.Everyday,
	DefenderScheduledScanTime = new Time(DateTime.Parse("11:59:10.9990000")),
	DefenderDetectedMalwareActions = new DefenderDetectedMalwareActions
	{
		OdataType = "microsoft.graph.defenderDetectedMalwareActions",
		LowSeverity = DefenderThreatAction.Clean,
		ModerateSeverity = DefenderThreatAction.Clean,
		HighSeverity = DefenderThreatAction.Clean,
		SevereSeverity = DefenderThreatAction.Clean,
	},
	DefenderFileExtensionsToExclude = new List<string>
	{
		"Defender File Extensions To Exclude value",
	},
	DefenderFilesAndFoldersToExclude = new List<string>
	{
		"Defender Files And Folders To Exclude value",
	},
	DefenderProcessesToExclude = new List<string>
	{
		"Defender Processes To Exclude value",
	},
	LockScreenAllowTimeoutConfiguration = true,
	LockScreenBlockActionCenterNotifications = true,
	LockScreenBlockCortana = true,
	LockScreenBlockToastNotifications = true,
	LockScreenTimeoutInSeconds = 10,
	PasswordBlockSimple = true,
	PasswordExpirationDays = 6,
	PasswordMinimumLength = 5,
	PasswordMinutesOfInactivityBeforeScreenTimeout = 14,
	PasswordMinimumCharacterSetCount = 0,
	PasswordPreviousPasswordBlockCount = 2,
	PasswordRequired = true,
	PasswordRequireWhenResumeFromIdleState = true,
	PasswordRequiredType = RequiredPasswordType.Alphanumeric,
	PasswordSignInFailureCountBeforeFactoryReset = 12,
	PrivacyAdvertisingId = StateManagementSetting.Blocked,
	PrivacyAutoAcceptPairingAndConsentPrompts = true,
	PrivacyBlockInputPersonalization = true,
	StartBlockUnpinningAppsFromTaskbar = true,
	StartMenuAppListVisibility = WindowsStartMenuAppListVisibilityType.Collapse,
	StartMenuHideChangeAccountSettings = true,
	StartMenuHideFrequentlyUsedApps = true,
	StartMenuHideHibernate = true,
	StartMenuHideLock = true,
	StartMenuHidePowerButton = true,
	StartMenuHideRecentJumpLists = true,
	StartMenuHideRecentlyAddedApps = true,
	StartMenuHideRestartOptions = true,
	StartMenuHideShutDown = true,
	StartMenuHideSignOut = true,
	StartMenuHideSleep = true,
	StartMenuHideSwitchAccount = true,
	StartMenuHideUserTile = true,
	StartMenuLayoutEdgeAssetsXml = Convert.FromBase64String("c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA=="),
	StartMenuLayoutXml = Convert.FromBase64String("c3RhcnRNZW51TGF5b3V0WG1s"),
	StartMenuMode = WindowsStartMenuModeType.FullScreen,
	StartMenuPinnedFolderDocuments = VisibilitySetting.Hide,
	StartMenuPinnedFolderDownloads = VisibilitySetting.Hide,
	StartMenuPinnedFolderFileExplorer = VisibilitySetting.Hide,
	StartMenuPinnedFolderHomeGroup = VisibilitySetting.Hide,
	StartMenuPinnedFolderMusic = VisibilitySetting.Hide,
	StartMenuPinnedFolderNetwork = VisibilitySetting.Hide,
	StartMenuPinnedFolderPersonalFolder = VisibilitySetting.Hide,
	StartMenuPinnedFolderPictures = VisibilitySetting.Hide,
	StartMenuPinnedFolderSettings = VisibilitySetting.Hide,
	StartMenuPinnedFolderVideos = VisibilitySetting.Hide,
	SettingsBlockSettingsApp = true,
	SettingsBlockSystemPage = true,
	SettingsBlockDevicesPage = true,
	SettingsBlockNetworkInternetPage = true,
	SettingsBlockPersonalizationPage = true,
	SettingsBlockAccountsPage = true,
	SettingsBlockTimeLanguagePage = true,
	SettingsBlockEaseOfAccessPage = true,
	SettingsBlockPrivacyPage = true,
	SettingsBlockUpdateSecurityPage = true,
	SettingsBlockAppsPage = true,
	SettingsBlockGamingPage = true,
	WindowsSpotlightBlockConsumerSpecificFeatures = true,
	WindowsSpotlightBlocked = true,
	WindowsSpotlightBlockOnActionCenter = true,
	WindowsSpotlightBlockTailoredExperiences = true,
	WindowsSpotlightBlockThirdPartyNotifications = true,
	WindowsSpotlightBlockWelcomeExperience = true,
	WindowsSpotlightBlockWindowsTips = true,
	WindowsSpotlightConfigureOnLockScreen = WindowsSpotlightEnablementSettings.Disabled,
	NetworkProxyApplySettingsDeviceWide = true,
	NetworkProxyDisableAutoDetect = true,
	NetworkProxyAutomaticConfigurationUrl = "https://example.com/networkProxyAutomaticConfigurationUrl/",
	NetworkProxyServer = new Windows10NetworkProxyServer
	{
		OdataType = "microsoft.graph.windows10NetworkProxyServer",
		Address = "Address value",
		Exceptions = new List<string>
		{
			"Exceptions value",
		},
		UseForLocalAddresses = true,
	},
	AccountsBlockAddingNonMicrosoftAccountEmail = true,
	AntiTheftModeBlocked = true,
	BluetoothBlocked = true,
	CameraBlocked = true,
	ConnectedDevicesServiceBlocked = true,
	CertificatesBlockManualRootCertificateInstallation = true,
	CopyPasteBlocked = true,
	CortanaBlocked = true,
	DeviceManagementBlockFactoryResetOnMobile = true,
	DeviceManagementBlockManualUnenroll = true,
	SafeSearchFilter = SafeSearchFilterType.Strict,
	EdgeBlockPopups = true,
	EdgeBlockSearchSuggestions = true,
	EdgeBlockSendingIntranetTrafficToInternetExplorer = true,
	EdgeSendIntranetTrafficToInternetExplorer = true,
	EdgeRequireSmartScreen = true,
	EdgeEnterpriseModeSiteListLocation = "Edge Enterprise Mode Site List Location value",
	EdgeFirstRunUrl = "https://example.com/edgeFirstRunUrl/",
	EdgeSearchEngine = new EdgeSearchEngineBase
	{
		OdataType = "microsoft.graph.edgeSearchEngineBase",
	},
	EdgeHomepageUrls = new List<string>
	{
		"Edge Homepage Urls value",
	},
	EdgeBlockAccessToAboutFlags = true,
	SmartScreenBlockPromptOverride = true,
	SmartScreenBlockPromptOverrideForFiles = true,
	WebRtcBlockLocalhostIpAddress = true,
	InternetSharingBlocked = true,
	SettingsBlockAddProvisioningPackage = true,
	SettingsBlockRemoveProvisioningPackage = true,
	SettingsBlockChangeSystemTime = true,
	SettingsBlockEditDeviceName = true,
	SettingsBlockChangeRegion = true,
	SettingsBlockChangeLanguage = true,
	SettingsBlockChangePowerSleep = true,
	LocationServicesBlocked = true,
	MicrosoftAccountBlocked = true,
	MicrosoftAccountBlockSettingsSync = true,
	NfcBlocked = true,
	ResetProtectionModeBlocked = true,
	ScreenCaptureBlocked = true,
	StorageBlockRemovableStorage = true,
	StorageRequireMobileDeviceEncryption = true,
	UsbBlocked = true,
	VoiceRecordingBlocked = true,
	WiFiBlockAutomaticConnectHotspots = true,
	WiFiBlocked = true,
	WiFiBlockManualConfiguration = true,
	WiFiScanInterval = 0,
	WirelessDisplayBlockProjectionToThisDevice = true,
	WirelessDisplayBlockUserInputFromReceiver = true,
	WirelessDisplayRequirePinForPairing = true,
	WindowsStoreBlocked = true,
	AppsAllowTrustedAppsSideloading = StateManagementSetting.Blocked,
	WindowsStoreBlockAutoUpdate = true,
	DeveloperUnlockSetting = StateManagementSetting.Blocked,
	SharedUserAppDataAllowed = true,
	AppsBlockWindowsStoreOriginatedApps = true,
	WindowsStoreEnablePrivateStoreOnly = true,
	StorageRestrictAppDataToSystemVolume = true,
	StorageRestrictAppInstallToSystemVolume = true,
	GameDvrBlocked = true,
	ExperienceBlockDeviceDiscovery = true,
	ExperienceBlockErrorDialogWhenNoSIM = true,
	ExperienceBlockTaskSwitcher = true,
	LogonBlockFastUserSwitching = true,
	TenantLockdownRequireNetworkDuringOutOfBoxExperience = true,
};
var result = await graphClient.DeviceManagement.DeviceConfigurations["{deviceConfiguration-id}"].PatchAsync(requestBody);


```