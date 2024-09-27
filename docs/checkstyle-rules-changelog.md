# 📝 Rules Changelog
The following are the changes made to original [sun_checks.xml](https://github.com/ittovate/.github/blob/main/config/checkstyle/sun_checks.xml) rules to produce our [sun_checks_custom.xml](https://github.com/ittovate/.github/blob/main/config/checkstyle/sun_checks_custom.xml) rules:

- Enable `@SuppressWarnings` to suppress the error of Considering the main spring class a utility class which is not.
- Remove `HideField` check due to Checklist considering the parameters in constructors/setters hide fields which is not happening.
- Set max line length to 120 (To match default IntelliJ IDEA formatting)
- Configure import order to match default IntelliJ IDEA formatter configuration (tested on v14):
  - Group of static imports is on the bottom.
  - Groups of non-static imports: all imports except of "javax" and "java", then "javax" and "java".
  - imports will be sorted in the groups.
  - Groups are separated by one blank line.
- Disable JavaDocs check for:
  - Packages.
  - Fields.
  - Getters, setters, and constructors.
- Remove `DesignForExtension` check for simplicity and we don't want warning about missing JavaDocs for getters.
- Remove `FinalParameters` check to avoid clutter code.
