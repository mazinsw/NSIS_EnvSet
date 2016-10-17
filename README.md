## NSIS_EnvSet
###### NSIS Environment Setting Plugin with unicode and x64 support

## Functions
```
Boolean :SetGlobalEnvironment Name Value UserVariable
String :GetEnvironmentVariable Name
Boolean :DeleteEnvironmentVariable Name
Boolean :AddVariableToPath Value
Boolean :DelVariableOfPath Value
```
## Install
copy NSIS_EnvSet.dll to NSIS\Plugins folder

## Examples
```
NSIS_EnvSet::SetGlobalEnvironment "MyFolder" "C:\MyFolder" 1
```

```
NSIS_EnvSet::GetEnvironmentVariable "MyFolder"
Pop $1
MessageBox MB_ICONINFORMATION $1
```

```
NSIS_EnvSet::DeleteEnvironmentVariable "MyFolder"
NSIS_EnvSet::AddVariableToPath "%MyFolder%\files"
NSIS_EnvSet::DelVariableOfPath "%MyFolder%\files"
```
## License

Please see the [license file](/LICENSE.txt) for more information.