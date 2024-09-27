# ⏬ Installation
1. Open IntelliJ plugins marketplace: `File > Settings > Plugins > Marketplace`.
2. Search for `Checkstyle-IDEA`, install it, and restart IntelliJ.
3. Copy [config directory](https://github.com/ittovate/.github/tree/main/config) to the project root (only if it doesn't exist already).
4. Install Maven plugin (If it's a Maven project):
```xml
 <plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-checkstyle-plugin</artifactId>
    <version>3.4.0</version>
    <configuration>
        <configLocation>config/checkstyle/sun_checks_custom.xml</configLocation>
        <consoleOutput>true</consoleOutput>
        <failsOnError>true</failsOnError>
        <linkXRef>false</linkXRef>
    </configuration>
</plugin>
```

# ⚙ Configuration
1. Open IntelliJ plugin settings: `File > Settings > Tools > Checkstyle`.
2. Change Scan Scope to `Only Java Sources (including tests)`.
3. Add our custom `Configuration File` by clicking `+` :
	1. Add description `Sun Check (Custom)`.
	2. Browse and select following configuration file: `config/checkstyle/sun_checks_custom.xml`.
	3. Click `Next > Next > Finish`.
	4. Mark the new configuration to add it before pressing `OK`.

# 🚀 Usage
1. Open the plugin (Usually left/bottom of the IDE).
2. Change rules to `Sun Check (Custom)`.
3. Click `Check Project` to detect all problems.

<div align="center">
  <img src="https://github.com/user-attachments/assets/fac8f6ed-7065-45b7-9cb8-d234159c866d" alt="image"/>
</div>

# 💡 Tips
- If the project is Spring, use `@SuppressWarnings("checkstyle:HideUtilityClassConstructor")` for entry point class (main).
- Maven plugin helps detect and solve issues by linting them and also can be used as pre-commit hook.
- Rules are modified to match IntelliJ default formatting so use hotkey `CTRL + ALT + L` to solve any checkstyle formatting issues.
- If interested in changed rules, Check [changelog](https://github.com/ittovate/.github/blob/main/docs/checkstyle-rules-changelog.md).
