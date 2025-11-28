# sf-token-introspect-custom-policy
Salesforce API Token Validation

# Notes
1. mvn install:install-file -Dfile=/Users/Userid/Documents/my-policies/local-maven-repo/mule-http-policy-transform-extension-3.1.0-mule-plugin.jar -DgroupId=com.mulesoft.anypoint -DartifactId=mule-http-policy-transform-extension -Dversion=3.1.0 -Dpackaging=jar
2. mvn deploy:deploy-file -Durl=file:///Users/Userid/Documents/my-policies/local-maven-repo -DgroupId=com.mulesoft.anypoint  -Dfile=/Users/polagani/Documents/my-policies/local-maven-repo/mule-http-policy-transform-extension-3.1.0-mule-plugin.jar
3. <dependencies>
		<dependency>
			<groupId>com.mulesoft.anypoint</groupId>
			<artifactId>mule-http-policy-transform-extension</artifactId>
			<version>3.1.0</version>

			<systemPath>/Users/polagani/Documents/my-policies/local-maven-repo/mule-http-policy-transform-extension-3.1.0-mule-plugin.jar</systemPath>
			<scope>system</scope>
			<classifier>mule-plugin</classifier>

			<exclusions>
				<exclusion>
					<groupId>org.mule.connectors</groupId>
					<artifactId>mule-http-connector</artifactId>
				</exclusion>
			</exclusions>

		</dependency>

		<dependency>
			<groupId>org.mule.connectors</groupId>
			<artifactId>mule-http-connector</artifactId>
			<version>1.7.2</version>
			<classifier>mule-plugin</classifier>
		</dependency>
	</dependencies>


4. 	<repository>
			<id>maven-repository</id>
			<url>file:///Users/polagani/Documents/my-policies/local-maven-repo</url>
		</repository>
