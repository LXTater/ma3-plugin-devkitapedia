# Global Functions (Object-Free API) [AI]
Pages for the grandMA3 global Lua functions that the manual documents with an example. All entries are `[P]` unless the page says otherwise: they were built from the manual and have not been probed on hardware. Where the manual contradicts itself the page carries `[?]`.

---

## Command line & output
[Cmd](Cmd) · [CmdIndirect](CmdIndirect) · [CmdIndirectWait](CmdIndirectWait) · [CmdObj](CmdObj) · [Echo](Echo) · [ErrEcho](ErrEcho) · [ErrPrintf](ErrPrintf) · [Printf](Printf) · [Import](Import) · [Export](Export) · [ExportCSV](ExportCSV) · [ExportJson](ExportJson)

---

## Objects, handles & addresses
[FromAddr](FromAddr) · [ToAddr](ToAddr) · [HandleToInt](HandleToInt) · [HandleToStr](HandleToStr) · [IntToHandle](IntToHandle) · [StrToHandle](StrToHandle) · [IsObjectValid](IsObjectValid) · [ObjectList](ObjectList) · [ClassExists](ClassExists) · [IsClassDerivedFrom](IsClassDerivedFrom) · [GetClassDerivationLevel](GetClassDerivationLevel) · [GetApiDescriptor](GetApiDescriptor) · [GetObjApiDescriptor](GetObjApiDescriptor) · [GetTokenName](GetTokenName) · [GetTokenNameByIndex](GetTokenNameByIndex)

---

## Root objects & show data
[Root](Root) · [ShowData](ShowData) · [ShowSettings](ShowSettings) · [DataPool](DataPool) · [MasterPool](MasterPool) · [Patch](Patch) · [Programmer](Programmer) · [ProgrammerPart](ProgrammerPart) · [Pult](Pult) · [ConfigTable](ConfigTable) · [DeviceConfiguration](DeviceConfiguration) · [DefaultDisplayPositions](DefaultDisplayPositions)

---

## Current / selected state
[CurrentEnvironment](CurrentEnvironment) · [CurrentExecPage](CurrentExecPage) · [CurrentProfile](CurrentProfile) · [CurrentScreenConfig](CurrentScreenConfig) · [CurrentUser](CurrentUser) · [GetCurrentCue](GetCurrentCue) · [GetExecutor](GetExecutor) · [SelectedFeature](SelectedFeature) · [SelectedLayout](SelectedLayout) · [SelectedSequence](SelectedSequence) · [SelectedTimecode](SelectedTimecode) · [SelectedTimer](SelectedTimer) · [GetSelectedAttribute](GetSelectedAttribute)

---

## Selection
[Selection](Selection) · [SelectionCount](SelectionCount) · [SelectionFirst](SelectionFirst) · [SelectionNext](SelectionNext)

---

## Variables
[AddonVars](AddonVars) · [GlobalVars](GlobalVars) · [UserVars](UserVars) · [GetVar](GetVar) · [SetVar](SetVar) · [DelVar](DelVar)

---

## Undo & hooks
[CreateUndo](CreateUndo) · [CloseUndo](CloseUndo) · [HookObjectChange](HookObjectChange) · [Unhook](Unhook) · [UnhookMultiple](UnhookMultiple) · [DumpAllHooks](DumpAllHooks)

---

## Fixtures, patch & channels
[AddFixtures](AddFixtures) · [CreateMultiPatch](CreateMultiPatch) · [CheckDMXCollision](CheckDMXCollision) · [CheckFIDCollision](CheckFIDCollision) · [FirstDmxModeFixture](FirstDmxModeFixture) · [FixtureType](FixtureType) · [GetSubfixture](GetSubfixture) · [GetSubfixtureCount](GetSubfixtureCount) · [GetAttributeByUIChannel](GetAttributeByUIChannel) · [GetAttributeCount](GetAttributeCount) · [GetAttributeIndex](GetAttributeIndex) · [GetChannelFunction](GetChannelFunction) · [GetChannelFunctionIndex](GetChannelFunctionIndex) · [GetRTChannel](GetRTChannel) · [GetRTChannelCount](GetRTChannelCount) · [GetRTChannels](GetRTChannels) · [GetUIChannelCount](GetUIChannelCount) · [GetUIChannelIndex](GetUIChannelIndex) · [GetUIChannels](GetUIChannels) · [GetPresetData](GetPresetData)

---

## DMX
[GetDMXUniverse](GetDMXUniverse) · [GetDMXValue](GetDMXValue)

---

## User interface & input
[Confirm](Confirm) · [MessageBox](MessageBox) · [TextInput](TextInput) · [CloseAllOverlays](CloseAllOverlays) · [DrawPointer](DrawPointer) · [GetButton](GetButton) · [GetDisplayByIndex](GetDisplayByIndex) · [GetDisplayCollect](GetDisplayCollect) · [GetFocus](GetFocus) · [GetFocusDisplay](GetFocusDisplay) · [GetScreenContent](GetScreenContent) · [GetTopModal](GetTopModal) · [GetTopOverlay](GetTopOverlay) · [GetUIObjectAtPosition](GetUIObjectAtPosition) · [KeyboardObj](KeyboardObj) · [MouseObj](MouseObj) · [TouchObj](TouchObj) · [SetBlockInput](SetBlockInput) · [SetLED](SetLED) · [FindTexture](FindTexture) · [GetSample](GetSample)

---

## Progress bars
[StartProgress](StartProgress) · [StopProgress](StopProgress) · [SetProgress](SetProgress) · [SetProgressRange](SetProgressRange) · [SetProgressText](SetProgressText) · [IncProgress](IncProgress)

---

## Files & paths
[DirList](DirList) · [FileExists](FileExists) · [GetPath](GetPath) · [GetPathOverrideFor](GetPathOverrideFor) · [GetPathSeparator](GetPathSeparator) · [GetPathType](GetPathType)

---

## Timing
[Time](Time) · [Timer](Timer)

---

## System & build info
[BuildDetails](BuildDetails) · [DeskLocked](DeskLocked) · [GetDebugFPS](GetDebugFPS) · [GetShowFileStatus](GetShowFileStatus) · [HostOS](HostOS) · [HostSubType](HostSubType) · [HostType](HostType) · [NeedShowSave](NeedShowSave) · [ReleaseType](ReleaseType) · [SerialNumber](SerialNumber) · [Version](Version)

---

## Worked Example
[Steamboat Willie Player](Steamboat-Willie-Player): a complete plugin using Cmd, ShowData, DataPool, Time and Printf together.

---

## See Also
[User Interface Overview](User-Interface-Overview) · [Simple Plugin Template](Simple-Plugin-Template)

*Generated with Claude Sonnet 5.5 with Medium effort. Based on the MA manual's Object-Free API index; not verified on hardware.*
