ORG:
4ea59a01ff6a454ea58be1556f913c1f
337F03A6734c412c990db4E0dfD1C663

Mule-Internal
Client ID:
c001452061d24e2d9c18023cdde7327d
Client Secret:
441b596967704D4B9C5B89614fA07ADe


Salt:
Client ID:
830f7d773e6e409bb5197057c1dafd3e
Client Secret:
C8aB08Ee94da4e249c382C7bce80C540


NonSalt:



OAuth: 
Access token URI
https://anypoint.mulesoft.com/accounts/oauth2/token
Authorization URI
https://anypoint.mulesoft.com/accounts/oauth2/authorize

Search clients: https://anypoint.mulesoft.com/accounts/api/clients/search
{
  "client_id": ["client1", "client2"]
}

GEt Single client: https://anypoint.mulesoft.com/accounts/api/clients/{clientId}


Invalidates and deletes the specified access token: https://anypoint.mulesoft.com/accounts/api/access_tokens/{access_token}

access revoke:
Get roles: https://anypoint.mulesoft.com/accounts/api/clients/{clientId}/roles/{roleId}
https://anypoint.mulesoft.com/accounts/api/connectedApplications/revoke

****store key value pair in object store V2
https://docs.mulesoft.com/object-store/osv2-apis#example-store-a-key-value-pair


based on header 
-custom policy which calls api to block the IP/redirect to a dummy response
-REST call to trigger it



Options:
1. No direct REST aPI has been provided in their docs to block an IP address but they have prebuilt policies to be configured and applied for a API either via GUI or programtically
2. IP blocking/whitelist policy via REST api  > ACL
3. custom policy to be created with a specific header to block a request


why license:
https://help.mulesoft.com/s/article/Failed-to-Download-mule-http-policy-transform-extension-Artifact

**Create Policy**
https://docs.mulesoft.com/api-manager/2.x/custom-policy-getting-started
1. Get groupID/OrgID from Accessmanagement>Org and run this in cmd prompt

mvn -Parchetype-repository archetype:generate -DarchetypeGroupId=org.mule.tools -DarchetypeArtifactId=api-gateway-custom-policy-archetype -DarchetypeVersion=1.2.0 -DgroupId=b487bf86-7ece-4bce-9e91-2378e6a615d9 -DartifactId=CustomRequestBlocker -Dversion=1.0.0-SNAPSHOT -Dpackage=mule-policy

2. Import the code in Anypoint Studio workspace.

3. mvn clean install
   mvn deploy
   
   
   
   how did my delivery help clients
leadership examples
dev examples
lack of resources
quick learning and great results of it