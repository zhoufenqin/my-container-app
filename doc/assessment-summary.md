<!--assessment-report-overview-->

# App Modernization Assessment Summary

**Target Azure Services**: Azure Kubernetes Service, Azure App Service, Azure Container Apps

## Overall Statistics

**Total Applications**: 2

**airsonic**:
- Mandatory: 593
- Potential: 23
- Optional: 598

**airsonic-main**:
- Mandatory: 593
- Potential: 23
- Optional: 598

> **Severity Levels Explained:**
> - **Mandatory**: The issue has to be resolved for the migration to be successful.
> - **Potential**: This issue may be blocking in some situations but not in others. These issues should be reviewed to determine whether a change is required or not.
> - **Optional**: The issue discovered is real issue fixing which could improve the app after migration, however it is not blocking.
> - **Information**: The issue was raised only for informational purpose and is not required to be resolved.

## Applications Summary

### airsonic
- **JDK Version**: 11
- **Frameworks**: Spring Boot, Spring
- **Languages**: Java, JavaScript
- **Build Tools**: Maven

**Key Findings**:
- **Mandatory Issues (593 violations)**:
  - <!--ruleid=azure-java-version-02000-->Legacy Java version (1 location found)
  - <!--ruleid=spring-boot-to-azure-spring-boot-version-01000-->Spring Boot version is low (10 locations found)
  - <!--ruleid=spring-framework-version-01000-->Spring Framework version out of support (10 locations found)
  - <!--ruleid=unsecure-network-protocol-00000-->Use of unsecured network protocols or URI libraries (319 locations found)
  - <!--ruleid=embedded-cache-15000-->Caching - Spring Boot Cache library (1 location found)
  - <!--ruleid=local-storage-00002-->File system - java.net.URL/URI (8 locations found)
  - <!--ruleid=local-storage-00006-->Apache Commons I/O (3 locations found)
  - <!--ruleid=local-storage-00004-->File system - 'file://' scheme (5 locations found)
  - <!--ruleid=localhost-http-00001-->Local HTTP Calls (10 locations found)
  - <!--ruleid=logging-0002-->Avoid File System Logging in Configuration (1 location found)
  - <!--ruleid=jni-native-code-00001-->Java Native Processes (7 locations found)
  - <!--ruleid=local-storage-00001-->File system - Java IO (14 locations found)
  - <!--ruleid=local-storage-00005-->File system - Java NIO (145 locations found)
  - <!--ruleid=hardcoded-ip-address-->Hardcoded IP Address (30 locations found)
  - <!--ruleid=java-11-deprecate-javaee-00001-->The java.annotation (Common Annotations) module has been removed from OpenJDK 11 (22 locations found)
  - <!--ruleid=java-19-deprecate-locale-00000-->Deprecation of Locale Class Constructors (3 locations found)
  - <!--ruleid=java-20-deprecate-net-00000-->java.net.URL Constructors Are Deprecated (4 locations found)
- **Potential Issues (23 violations)**:
  - <!--ruleid=azure-password-01000-->Password found in configuration file (1 location found)
  - <!--ruleid=auth-02000-->Embedded framework - Spring Security (2 locations found)
  - <!--ruleid=azure-database-postgresql-02000-->PostgreSQL database found (2 locations found)
  - <!--ruleid=azure-database-mysql-01000-->MySQL database found (2 locations found)
  - <!--ruleid=mail-00000-->Java Mail API (5 locations found)
  - <!--ruleid=utf-8-by-default-00000-->The 'java.io' constructor defaults to UTF-8 (2 locations found)
  - <!--ruleid=utf-8-by-default-00020-->The java.net.URLEncoder.encode method uses UTF-8 by default (3 locations found)
  - <!--ruleid=utf-8-by-default-00030-->The java.net.URLDecoder.decode method uses UTF-8 by default (2 locations found)
  - <!--ruleid=oracle2openjdk-00004-->Java 2D library usage (2 locations found)
  - <!--ruleid=oracle2openjdk-00003-->Color management usage (2 locations found)
- **Optional Issues (598 violations)**:
  - <!--ruleid=java-ldap-to-msft-entra-id-01000-->Java LDAP usage detected (11 locations found)
  - <!--ruleid=azure-system-config-01000-->Environment variables/system properties (11 locations found)
  - <!--ruleid=database-reliability-01000-->Consider database reliability when migrating to Azure (1 location found)
  - <!--ruleid=jakarta-ee-version-01000-->Jakarta EE version not latest stable (1 location found)
  - <!--ruleid=socket-communication-00000-->Socket communication (1 location found)
  - <!--ruleid=hardcoded-urls-00001-->Avoid using hardcoded URLs (HTTP protocol) in source code (571 locations found)
  - <!--ruleid=hardcoded-urls-00002-->Avoid using hardcoded URLs (LDAP protocol) in source code (2 locations found)

### airsonic-main
- **JDK Version**: 11
- **Frameworks**: Spring Boot, Spring
- **Languages**: Java, JavaScript
- **Build Tools**: Maven

**Key Findings**:
- **Mandatory Issues (593 violations)**:
  - <!--ruleid=azure-java-version-02000-->Legacy Java version (1 location found)
  - <!--ruleid=spring-boot-to-azure-spring-boot-version-01000-->Spring Boot version is low (10 locations found)
  - <!--ruleid=spring-framework-version-01000-->Spring Framework version out of support (10 locations found)
  - <!--ruleid=unsecure-network-protocol-00000-->Use of unsecured network protocols or URI libraries (319 locations found)
  - <!--ruleid=embedded-cache-15000-->Caching - Spring Boot Cache library (1 location found)
  - <!--ruleid=local-storage-00002-->File system - java.net.URL/URI (8 locations found)
  - <!--ruleid=local-storage-00006-->Apache Commons I/O (3 locations found)
  - <!--ruleid=local-storage-00004-->File system - 'file://' scheme (5 locations found)
  - <!--ruleid=localhost-http-00001-->Local HTTP Calls (10 locations found)
  - <!--ruleid=logging-0002-->Avoid File System Logging in Configuration (1 location found)
  - <!--ruleid=jni-native-code-00001-->Java Native Processes (7 locations found)
  - <!--ruleid=local-storage-00001-->File system - Java IO (14 locations found)
  - <!--ruleid=local-storage-00005-->File system - Java NIO (145 locations found)
  - <!--ruleid=hardcoded-ip-address-->Hardcoded IP Address (30 locations found)
  - <!--ruleid=java-11-deprecate-javaee-00001-->The java.annotation (Common Annotations) module has been removed from OpenJDK 11 (22 locations found)
  - <!--ruleid=java-19-deprecate-locale-00000-->Deprecation of Locale Class Constructors (3 locations found)
  - <!--ruleid=java-20-deprecate-net-00000-->java.net.URL Constructors Are Deprecated (4 locations found)
- **Potential Issues (23 violations)**:
  - <!--ruleid=azure-password-01000-->Password found in configuration file (1 location found)
  - <!--ruleid=auth-02000-->Embedded framework - Spring Security (2 locations found)
  - <!--ruleid=azure-database-postgresql-02000-->PostgreSQL database found (2 locations found)
  - <!--ruleid=azure-database-mysql-01000-->MySQL database found (2 locations found)
  - <!--ruleid=mail-00000-->Java Mail API (5 locations found)
  - <!--ruleid=utf-8-by-default-00000-->The 'java.io' constructor defaults to UTF-8 (2 locations found)
  - <!--ruleid=utf-8-by-default-00020-->The java.net.URLEncoder.encode method uses UTF-8 by default (3 locations found)
  - <!--ruleid=utf-8-by-default-00030-->The java.net.URLDecoder.decode method uses UTF-8 by default (2 locations found)
  - <!--ruleid=oracle2openjdk-00004-->Java 2D library usage (2 locations found)
  - <!--ruleid=oracle2openjdk-00003-->Color management usage (2 locations found)
- **Optional Issues (598 violations)**:
  - <!--ruleid=java-ldap-to-msft-entra-id-01000-->Java LDAP usage detected (11 locations found)
  - <!--ruleid=azure-system-config-01000-->Environment variables/system properties (11 locations found)
  - <!--ruleid=database-reliability-01000-->Consider database reliability when migrating to Azure (1 location found)
  - <!--ruleid=jakarta-ee-version-01000-->Jakarta EE version not latest stable (1 location found)
  - <!--ruleid=socket-communication-00000-->Socket communication (1 location found)
  - <!--ruleid=hardcoded-urls-00001-->Avoid using hardcoded URLs (HTTP protocol) in source code (571 locations found)
  - <!--ruleid=hardcoded-urls-00002-->Avoid using hardcoded URLs (LDAP protocol) in source code (2 locations found)

## Next Steps

For comprehensive migration guidance and best practices, visit:
- [View Full Assessment Report](https://github.com/zhoufenqin/my-container-app/blob/assessment-reports/.github/appmod/appcat/issue-35-report.json)
- [GitHub Copilot App Modernization](https://learn.microsoft.com/en-us/azure/developer/java/migration/migrate-github-copilot-app-modernization-for-java)

