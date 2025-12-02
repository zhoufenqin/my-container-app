<!--assessment-report-overview-->

# App Modernization Assessment Summary

**Target Azure Services**: Azure Kubernetes Service, Azure App Service, Azure Container Apps

## Overall Statistics

**Total Applications**: 2

**Name: airsonic**
- Azure Kubernetes Service: 17 Mandatory, 10 Potential, 7 Optional
- Azure App Service: 17 Mandatory, 10 Potential, 7 Optional
- Azure Container Apps: 17 Mandatory, 10 Potential, 7 Optional

**Name: airsonic-main**
- Azure Kubernetes Service: 17 Mandatory, 10 Potential, 7 Optional
- Azure App Service: 17 Mandatory, 10 Potential, 7 Optional
- Azure Container Apps: 17 Mandatory, 10 Potential, 7 Optional

> **Severity Levels Explained:**
> - **Mandatory**: The issue has to be resolved for the migration to be successful.
> - **Potential**: This issue may be blocking in some situations but not in others. These issues should be reviewed to determine whether a change is required or not.
> - **Optional**: The issue discovered is real issue fixing which could improve the app after migration, however it is not blocking.

## Applications Profile

### Name: airsonic
- **JDK Version**: 11
- **Frameworks**: Spring Boot, Spring
- **Languages**: Java, JavaScript
- **Build Tools**: Maven

**Key Findings**:

- <details>
  <summary><!--ruleid=azure-database-mysql-01000--><b>MySQL database found</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure Database for MySQL documentation](https://learn.microsoft.com/azure/mysql), [Azure Database Migration Service documentation](https://learn.microsoft.com/azure/dms), [Azure Monitor documentation](https://learn.microsoft.com/azure/azure-monitor), [Microsoft Defender for Cloud](https://learn.microsoft.com/azure/defender-for-cloud), [Backup and restore in Azure Database for MySQL](https://learn.microsoft.com/azure/mysql/single-server/concepts-backup)

- <details>
  <summary><!--ruleid=spring-framework-version-01000--><b>Spring Framework Version End of OSS Support</b> (10 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Spring Framework Supported Versions](https://spring.io/projects/spring-framework#support), [Spring Framework Support Policy](https://github.com/spring-projects/spring-framework/wiki/Spring-Framework-Versions)

- <details>
  <summary><!--ruleid=java-ldap-to-msft-entra-id-01000--><b>Java LDAP usage detected</b> (11 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>
  
  **Links**: [What is Microsoft Entra ID?](https://learn.microsoft.com/en-us/entra/fundamentals/whatis)

- <details>
  <summary><!--ruleid=spring-boot-to-azure-spring-boot-version-01000--><b>Spring Boot Version is End of OSS Support</b> (10 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 5
  - Azure App Service: mandatory, Effort: 5
  - Azure Container Apps: mandatory, Effort: 5
  </details>
  
  **Links**: [Migrate Spring Boot applications to Azure Container Apps](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-azure-container-apps), [Launch your first Java microservice application with managed Java components in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/java-microservice-get-started?tabs=azure-cli), [Spring Boot Supported Versions](https://spring.io/projects/spring-boot/#support), [Spring Boot Support Policy](https://github.com/spring-projects/spring-boot/wiki/Supported-Versions)

- <details>
  <summary><!--ruleid=database-reliability-01000--><b>Consider database reliability when migrating to Azure</b> (1 location)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>
  
  **Links**: [Understanding timeout properties in the JDBC driver](https://learn.microsoft.com/sql/connect/jdbc/understand-timeouts), [Setting the connection properties](https://learn.microsoft.com/sql/connect/jdbc/setting-the-connection-properties), [Managing transaction size](https://learn.microsoft.com/sql/connect/jdbc/managing-transaction-size), [Retry pattern](https://learn.microsoft.com/azure/architecture/patterns/retry), [Implementing retries with exponential backoff](https://www.learntocodetogether.com/retry-exponential-back-off/), [Transient fault handling](https://learn.microsoft.com/azure/architecture/best-practices/transient-faults)

- <details>
  <summary><!--ruleid=azure-password-01000--><b>Password found in configuration file</b> (1 location)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure Key Vault documentation](https://learn.microsoft.com/azure/key-vault), [Passwordless connections for Azure services](https://learn.microsoft.com/azure/developer/intro/passwordless-overview), [Password found in configuration file](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-azure-container-apps#inventory-configuration-sources-and-secrets), [Read a secret from Azure Key Vault in a Spring Boot application](https://docs.microsoft.com/azure/developer/java/spring-framework/configure-spring-boot-starter-java-app-with-azure-key-vault), [Azure Spring Boot Starter for Azure Key Vault Secrets](https://search.maven.org/artifact/com.azure.spring/azure-spring-boot-starter-keyvault-secrets)

- <details>
  <summary><!--ruleid=auth-02000--><b>Embedded framework - Spring Security</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [Spring Security-related dependencies found in the project](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-app-service#identity-providers), [Azure Active Directory (Azure AD) identity provider for External Identities](https://docs.microsoft.com/azure/active-directory/external-identities/azure-ad-account), [Spring Security](https://docs.spring.io/spring-security/reference/index.html), [Spring Boot API: Authorization](https://auth0.com/docs/quickstart/backend/java-spring-security5/01-authorization)

- <details>
  <summary><!--ruleid=jakarta-ee-version-01000--><b>Jakarta EE version not latest stable</b> (1 location)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>
  
  **Links**: [Jakarta EE Release Versions](https://jakarta.ee/release/), [Jakarta EE Platforms](https://jakarta.ee/specifications/platform/)

- <details>
  <summary><!--ruleid=azure-java-version-02000--><b>Legacy Java version</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=azure-system-config-01000--><b>Environment variables/system properties</b> (11 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 1
  - Azure App Service: optional, Effort: 1
  - Azure Container Apps: optional, Effort: 1
  </details>
  
  **Links**: [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration), [Azure Key Vault documentation](https://learn.microsoft.com/azure/key-vault), [Configure per-service secrets and externalized settings](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-azure-container-apps#configure-per-service-secrets-and-externalized-settings)

- <details>
  <summary><!--ruleid=azure-database-postgresql-02000--><b>PostgreSQL database found</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure PostgreSQL Flexible Server documentation](https://learn.microsoft.com/azure/postgresql/flexible-server), [Azure Database Migration Service documentation](https://learn.microsoft.com/azure/dms), [Azure Monitor documentation](https://learn.microsoft.com/azure/azure-monitor), [Microsoft Defender for Cloud](https://learn.microsoft.com/azure/defender-for-cloud), [Backup and restore in Azure Database for PostgreSQL](https://learn.microsoft.com/azure/postgresql/single-server/concepts-backup)

- <details>
  <summary><!--ruleid=embedded-cache-15000--><b>Caching - Spring Boot Cache library</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 5
  - Azure App Service: mandatory, Effort: 5
  - Azure Container Apps: mandatory, Effort: 5
  </details>

- <details>
  <summary><!--ruleid=jni-native-code-00001--><b>Java Native Processes</b> (7 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 7
  - Azure App Service: mandatory, Effort: 7
  - Azure Container Apps: mandatory, Effort: 7
  </details>
  
  **Links**: [Advanced example for containers](https://docs.microsoft.com/en-us/visualstudio/install/advanced-build-tools-container?view=vs-2019), [how to register com components inside docker as regsvr32 command](https://stackoverflow.com/questions/54502335/how-to-register-com-components-inside-docker-as-regsvr32-command-executes-succes), [How to containerize the .NET Framework web apps with Windows Containers and Docker](https://github.com/dotnet-architecture/eShopModernizing/wiki/02.-How-to-containerize-the-.NET-Framework-web-apps-with-Windows-Containers-and-Docker), [Windows Application 32 bit COM dll registration](https://forums.docker.com/t/windows-application-32-bit-com-dll-registration/47205/8)

- <details>
  <summary><!--ruleid=local-storage-00001--><b>File system - Java IO</b> (14 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Azure Storage documentation](https://learn.microsoft.com/azure/storage), [Create an Azure Files volume mount in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts-azure-files), [Use storage mounts in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts), [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Azure Cache for Redis documentation](https://learn.microsoft.com/azure/azure-cache-for-redis), [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration)

- <details>
  <summary><!--ruleid=localhost-http-00001--><b>Local HTTP Calls</b> (10 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 7
  - Azure App Service: mandatory, Effort: 7
  - Azure Container Apps: mandatory, Effort: 7
  </details>

- <details>
  <summary><!--ruleid=socket-communication-00000--><b>Socket communication</b> (1 location)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 5
  - Azure App Service: optional, Effort: 5
  - Azure Container Apps: optional, Effort: 5
  </details>

- <details>
  <summary><!--ruleid=mail-00000--><b>Java Mail API</b> (5 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure Communication Services documentation](https://learn.microsoft.com/azure/communication-services), [Quickstart: How to send an email using Azure Communication Service](https://learn.microsoft.com/azure/communication-services/quickstarts/email/send-email), [Troubleshoot outbound SMTP connectivity problems in Azure](https://learn.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)

- <details>
  <summary><!--ruleid=local-storage-00002--><b>File system - java.net.URL/URI</b> (8 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Azure Storage documentation](https://learn.microsoft.com/azure/storage), [Create an Azure Files volume mount in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts-azure-files), [Use storage mounts in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts), [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Azure Cache for Redis documentation](https://learn.microsoft.com/azure/azure-cache-for-redis), [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration)

- <details>
  <summary><!--ruleid=local-storage-00006--><b>Apache Commons I/O</b> (3 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=local-storage-00005--><b>File system - Java NIO</b> (145 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=local-storage-00004--><b>File system - 'file://' scheme</b> (5 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Azure Storage documentation](https://learn.microsoft.com/azure/storage), [Create an Azure Files volume mount in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts-azure-files), [Use storage mounts in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts), [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Azure Cache for Redis documentation](https://learn.microsoft.com/azure/azure-cache-for-redis), [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration)

- <details>
  <summary><!--ruleid=logging-0002--><b>Avoid File System Logging in Configuration</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure App Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Log queries in Azure Monitor](https://learn.microsoft.com/azure/azure-monitor/logs/log-query-overview), [Enable diagnostics logging for apps in Azure App Service](https://learn.microsoft.com/azure/app-service/troubleshoot-diagnostic-logs), [Log Analytics tutorial](https://learn.microsoft.com/azure/azure-monitor/logs/log-analytics-tutorial)

- <details>
  <summary><!--ruleid=hardcoded-urls-00001--><b>Avoid using hardcoded URLs (HTTP protocol) in source code</b> (571 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=hardcoded-urls-00002--><b>Avoid using hardcoded URLs (LDAP protocol) in source code</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=unsecure-network-protocol-00000--><b>Use of unsecured network protocols or URI libraries</b> (319 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Why HTTPS matters](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/why-https), [SSH File Transfer Protocol (SFTP): Get SFTP client & server](https://www.ssh.com/ssh/sftp/)

- <details>
  <summary><!--ruleid=hardcoded-ip-address--><b>Hardcoded IP Address</b> (30 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=java-11-deprecate-javaee-00001--><b>The java.annotation (Common Annotations) module has been removed from OpenJDK 11</b> (22 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure App Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Removed Java EE modules](https://www.oracle.com/java/technologies/javase/11-relnote-issues.html#JDK-8190378)

- <details>
  <summary><!--ruleid=java-20-deprecate-net-00000--><b>java.net.URL Constructors Are Deprecated</b> (4 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [java.net.URL Constructors Are Deprecated](https://www.oracle.com/java/technologies/javase/20-relnote-issues.html#JDK-8294241)

- <details>
  <summary><!--ruleid=utf-8-by-default-00000--><b>The 'java.io' constructor defaults to UTF-8</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [JEP 400: UTF-8 by Default](https://openjdk.org/jeps/400)

- <details>
  <summary><!--ruleid=utf-8-by-default-00020--><b>The java.net.URLEncoder.encode method uses UTF-8 by default</b> (3 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [JEP 400: UTF-8 by Default](https://openjdk.org/jeps/400)

- <details>
  <summary><!--ruleid=utf-8-by-default-00030--><b>The java.net.URLDecoder.decode method uses UTF-8 by default</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [JEP 400: UTF-8 by Default](https://openjdk.org/jeps/400)

- <details>
  <summary><!--ruleid=java-19-deprecate-locale-00000--><b>Deprecation of Locale Class Constructors</b> (3 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure App Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Deprecation of Locale Class Constructors](https://www.oracle.com/java/technologies/javase/19-relnote-issues.html#JDK-8282819)

- <details>
  <summary><!--ruleid=oracle2openjdk-00004--><b>Java 2D library usage</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [Knowledge base article OracleJDK vs. OpenJDK](https://access.redhat.com/solutions/2489791)

- <details>
  <summary><!--ruleid=oracle2openjdk-00003--><b>Color management usage</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [Knowledge base article OracleJDK vs. OpenJDK](https://access.redhat.com/solutions/2489791)

### Name: airsonic-main
- **JDK Version**: 11
- **Frameworks**: Spring Boot, Spring
- **Languages**: Java, JavaScript
- **Build Tools**: Maven

**Key Findings**:

- <details>
  <summary><!--ruleid=azure-database-mysql-01000--><b>MySQL database found</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure Database for MySQL documentation](https://learn.microsoft.com/azure/mysql), [Azure Database Migration Service documentation](https://learn.microsoft.com/azure/dms), [Azure Monitor documentation](https://learn.microsoft.com/azure/azure-monitor), [Microsoft Defender for Cloud](https://learn.microsoft.com/azure/defender-for-cloud), [Backup and restore in Azure Database for MySQL](https://learn.microsoft.com/azure/mysql/single-server/concepts-backup)

- <details>
  <summary><!--ruleid=spring-framework-version-01000--><b>Spring Framework Version End of OSS Support</b> (10 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Spring Framework Supported Versions](https://spring.io/projects/spring-framework#support), [Spring Framework Support Policy](https://github.com/spring-projects/spring-framework/wiki/Spring-Framework-Versions)

- <details>
  <summary><!--ruleid=java-ldap-to-msft-entra-id-01000--><b>Java LDAP usage detected</b> (11 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>
  
  **Links**: [What is Microsoft Entra ID?](https://learn.microsoft.com/en-us/entra/fundamentals/whatis)

- <details>
  <summary><!--ruleid=spring-boot-to-azure-spring-boot-version-01000--><b>Spring Boot Version is End of OSS Support</b> (10 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 5
  - Azure App Service: mandatory, Effort: 5
  - Azure Container Apps: mandatory, Effort: 5
  </details>
  
  **Links**: [Migrate Spring Boot applications to Azure Container Apps](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-azure-container-apps), [Launch your first Java microservice application with managed Java components in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/java-microservice-get-started?tabs=azure-cli), [Spring Boot Supported Versions](https://spring.io/projects/spring-boot/#support), [Spring Boot Support Policy](https://github.com/spring-projects/spring-boot/wiki/Supported-Versions)

- <details>
  <summary><!--ruleid=database-reliability-01000--><b>Consider database reliability when migrating to Azure</b> (1 location)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>
  
  **Links**: [Understanding timeout properties in the JDBC driver](https://learn.microsoft.com/sql/connect/jdbc/understand-timeouts), [Setting the connection properties](https://learn.microsoft.com/sql/connect/jdbc/setting-the-connection-properties), [Managing transaction size](https://learn.microsoft.com/sql/connect/jdbc/managing-transaction-size), [Retry pattern](https://learn.microsoft.com/azure/architecture/patterns/retry), [Implementing retries with exponential backoff](https://www.learntocodetogether.com/retry-exponential-back-off/), [Transient fault handling](https://learn.microsoft.com/azure/architecture/best-practices/transient-faults)

- <details>
  <summary><!--ruleid=azure-password-01000--><b>Password found in configuration file</b> (1 location)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure Key Vault documentation](https://learn.microsoft.com/azure/key-vault), [Passwordless connections for Azure services](https://learn.microsoft.com/azure/developer/intro/passwordless-overview), [Password found in configuration file](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-azure-container-apps#inventory-configuration-sources-and-secrets), [Read a secret from Azure Key Vault in a Spring Boot application](https://docs.microsoft.com/azure/developer/java/spring-framework/configure-spring-boot-starter-java-app-with-azure-key-vault), [Azure Spring Boot Starter for Azure Key Vault Secrets](https://search.maven.org/artifact/com.azure.spring/azure-spring-boot-starter-keyvault-secrets)

- <details>
  <summary><!--ruleid=auth-02000--><b>Embedded framework - Spring Security</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [Spring Security-related dependencies found in the project](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-app-service#identity-providers), [Azure Active Directory (Azure AD) identity provider for External Identities](https://docs.microsoft.com/azure/active-directory/external-identities/azure-ad-account), [Spring Security](https://docs.spring.io/spring-security/reference/index.html), [Spring Boot API: Authorization](https://auth0.com/docs/quickstart/backend/java-spring-security5/01-authorization)

- <details>
  <summary><!--ruleid=jakarta-ee-version-01000--><b>Jakarta EE version not latest stable</b> (1 location)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>
  
  **Links**: [Jakarta EE Release Versions](https://jakarta.ee/release/), [Jakarta EE Platforms](https://jakarta.ee/specifications/platform/)

- <details>
  <summary><!--ruleid=azure-java-version-02000--><b>Legacy Java version</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=azure-system-config-01000--><b>Environment variables/system properties</b> (11 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 1
  - Azure App Service: optional, Effort: 1
  - Azure Container Apps: optional, Effort: 1
  </details>
  
  **Links**: [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration), [Azure Key Vault documentation](https://learn.microsoft.com/azure/key-vault), [Configure per-service secrets and externalized settings](https://learn.microsoft.com/azure/developer/java/migration/migrate-spring-boot-to-azure-container-apps#configure-per-service-secrets-and-externalized-settings)

- <details>
  <summary><!--ruleid=azure-database-postgresql-02000--><b>PostgreSQL database found</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure PostgreSQL Flexible Server documentation](https://learn.microsoft.com/azure/postgresql/flexible-server), [Azure Database Migration Service documentation](https://learn.microsoft.com/azure/dms), [Azure Monitor documentation](https://learn.microsoft.com/azure/azure-monitor), [Microsoft Defender for Cloud](https://learn.microsoft.com/azure/defender-for-cloud), [Backup and restore in Azure Database for PostgreSQL](https://learn.microsoft.com/azure/postgresql/single-server/concepts-backup)

- <details>
  <summary><!--ruleid=embedded-cache-15000--><b>Caching - Spring Boot Cache library</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 5
  - Azure App Service: mandatory, Effort: 5
  - Azure Container Apps: mandatory, Effort: 5
  </details>

- <details>
  <summary><!--ruleid=jni-native-code-00001--><b>Java Native Processes</b> (7 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 7
  - Azure App Service: mandatory, Effort: 7
  - Azure Container Apps: mandatory, Effort: 7
  </details>
  
  **Links**: [Advanced example for containers](https://docs.microsoft.com/en-us/visualstudio/install/advanced-build-tools-container?view=vs-2019), [how to register com components inside docker as regsvr32 command](https://stackoverflow.com/questions/54502335/how-to-register-com-components-inside-docker-as-regsvr32-command-executes-succes), [How to containerize the .NET Framework web apps with Windows Containers and Docker](https://github.com/dotnet-architecture/eShopModernizing/wiki/02.-How-to-containerize-the-.NET-Framework-web-apps-with-Windows-Containers-and-Docker), [Windows Application 32 bit COM dll registration](https://forums.docker.com/t/windows-application-32-bit-com-dll-registration/47205/8)

- <details>
  <summary><!--ruleid=local-storage-00001--><b>File system - Java IO</b> (14 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Azure Storage documentation](https://learn.microsoft.com/azure/storage), [Create an Azure Files volume mount in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts-azure-files), [Use storage mounts in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts), [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Azure Cache for Redis documentation](https://learn.microsoft.com/azure/azure-cache-for-redis), [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration)

- <details>
  <summary><!--ruleid=localhost-http-00001--><b>Local HTTP Calls</b> (10 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 7
  - Azure App Service: mandatory, Effort: 7
  - Azure Container Apps: mandatory, Effort: 7
  </details>

- <details>
  <summary><!--ruleid=socket-communication-00000--><b>Socket communication</b> (1 location)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 5
  - Azure App Service: optional, Effort: 5
  - Azure Container Apps: optional, Effort: 5
  </details>

- <details>
  <summary><!--ruleid=mail-00000--><b>Java Mail API</b> (5 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 3
  - Azure App Service: potential, Effort: 3
  - Azure Container Apps: potential, Effort: 3
  </details>
  
  **Links**: [Azure Communication Services documentation](https://learn.microsoft.com/azure/communication-services), [Quickstart: How to send an email using Azure Communication Service](https://learn.microsoft.com/azure/communication-services/quickstarts/email/send-email), [Troubleshoot outbound SMTP connectivity problems in Azure](https://learn.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)

- <details>
  <summary><!--ruleid=local-storage-00002--><b>File system - java.net.URL/URI</b> (8 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Azure Storage documentation](https://learn.microsoft.com/azure/storage), [Create an Azure Files volume mount in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts-azure-files), [Use storage mounts in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts), [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Azure Cache for Redis documentation](https://learn.microsoft.com/azure/azure-cache-for-redis), [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration)

- <details>
  <summary><!--ruleid=local-storage-00006--><b>Apache Commons I/O</b> (3 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=local-storage-00005--><b>File system - Java NIO</b> (145 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=local-storage-00004--><b>File system - 'file://' scheme</b> (5 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Azure Storage documentation](https://learn.microsoft.com/azure/storage), [Create an Azure Files volume mount in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts-azure-files), [Use storage mounts in Azure Container Apps](https://learn.microsoft.com/azure/container-apps/storage-mounts), [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Azure Cache for Redis documentation](https://learn.microsoft.com/azure/azure-cache-for-redis), [Azure App Configuration documentation](https://learn.microsoft.com/azure/azure-app-configuration)

- <details>
  <summary><!--ruleid=logging-0002--><b>Avoid File System Logging in Configuration</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure App Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Azure Monitor Logs overview](https://learn.microsoft.com/azure/azure-monitor/logs/data-platform-logs), [Log queries in Azure Monitor](https://learn.microsoft.com/azure/azure-monitor/logs/log-query-overview), [Enable diagnostics logging for apps in Azure App Service](https://learn.microsoft.com/azure/app-service/troubleshoot-diagnostic-logs), [Log Analytics tutorial](https://learn.microsoft.com/azure/azure-monitor/logs/log-analytics-tutorial)

- <details>
  <summary><!--ruleid=hardcoded-urls-00001--><b>Avoid using hardcoded URLs (HTTP protocol) in source code</b> (571 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=hardcoded-urls-00002--><b>Avoid using hardcoded URLs (LDAP protocol) in source code</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: optional, Effort: 3
  - Azure App Service: optional, Effort: 3
  - Azure Container Apps: optional, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=unsecure-network-protocol-00000--><b>Use of unsecured network protocols or URI libraries</b> (319 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [Why HTTPS matters](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/why-https), [SSH File Transfer Protocol (SFTP): Get SFTP client & server](https://www.ssh.com/ssh/sftp/)

- <details>
  <summary><!--ruleid=hardcoded-ip-address--><b>Hardcoded IP Address</b> (30 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>

- <details>
  <summary><!--ruleid=java-11-deprecate-javaee-00001--><b>The java.annotation (Common Annotations) module has been removed from OpenJDK 11</b> (22 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure App Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Removed Java EE modules](https://www.oracle.com/java/technologies/javase/11-relnote-issues.html#JDK-8190378)

- <details>
  <summary><!--ruleid=java-20-deprecate-net-00000--><b>java.net.URL Constructors Are Deprecated</b> (4 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 3
  - Azure App Service: mandatory, Effort: 3
  - Azure Container Apps: mandatory, Effort: 3
  </details>
  
  **Links**: [java.net.URL Constructors Are Deprecated](https://www.oracle.com/java/technologies/javase/20-relnote-issues.html#JDK-8294241)

- <details>
  <summary><!--ruleid=utf-8-by-default-00000--><b>The 'java.io' constructor defaults to UTF-8</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [JEP 400: UTF-8 by Default](https://openjdk.org/jeps/400)

- <details>
  <summary><!--ruleid=utf-8-by-default-00020--><b>The java.net.URLEncoder.encode method uses UTF-8 by default</b> (3 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [JEP 400: UTF-8 by Default](https://openjdk.org/jeps/400)

- <details>
  <summary><!--ruleid=utf-8-by-default-00030--><b>The java.net.URLDecoder.decode method uses UTF-8 by default</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [JEP 400: UTF-8 by Default](https://openjdk.org/jeps/400)

- <details>
  <summary><!--ruleid=java-19-deprecate-locale-00000--><b>Deprecation of Locale Class Constructors</b> (3 locations)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure App Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Deprecation of Locale Class Constructors](https://www.oracle.com/java/technologies/javase/19-relnote-issues.html#JDK-8282819)

- <details>
  <summary><!--ruleid=oracle2openjdk-00004--><b>Java 2D library usage</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [Knowledge base article OracleJDK vs. OpenJDK](https://access.redhat.com/solutions/2489791)

- <details>
  <summary><!--ruleid=oracle2openjdk-00003--><b>Color management usage</b> (2 locations)</summary>
  
  - Azure Kubernetes Service: potential, Effort: 1
  - Azure App Service: potential, Effort: 1
  - Azure Container Apps: potential, Effort: 1
  </details>
  
  **Links**: [Knowledge base article OracleJDK vs. OpenJDK](https://access.redhat.com/solutions/2489791)

## General Key Findings

- <details>
  <summary><!--ruleid=dockerfile-00000--><b>No Dockerfile found</b> (1 location)</summary>
  
  - Azure Kubernetes Service: mandatory, Effort: 1
  - Azure Container Apps: mandatory, Effort: 1
  </details>
  
  **Links**: [Dockerizing a Java Application](https://www.baeldung.com/java-dockerize-app)

## Next Steps

For comprehensive migration guidance and best practices, visit:
- [GitHub Copilot App Modernization](https://aka.ms/ghcp-appmod)
