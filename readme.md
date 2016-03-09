# Without KB3135996

```
Signing: http://www.microsoft.com
XML Signature was succesfully computed and saved to xmldsig.xml.
Verifying signature...
The XML signature is valid.
```

# With KB3135996

```
Signing: http://www.microsoft.com
System.Security.Cryptography.CryptographicException: Unable to resolve Uri http://www.microsoft.com.
   at System.Security.Cryptography.Xml.Reference.CalculateHashValue(XmlDocument document, CanonicalXmlNodeList refList)
   at System.Security.Cryptography.Xml.SignedXml.BuildDigestedReferences()
   at System.Security.Cryptography.Xml.SignedXml.ComputeSignature()
   at SigningTest.Program.SignDetachedResource(String URIString, String XmlSigFileName, RSA Key) in c:\temp\sig2\.NET-Sign-CryptographicException\SigningTest\Program.cs:line 88
   at SigningTest.Program.Main(String[] args) in c:\temp\sig2\.NET-Sign-CryptographicException\SigningTest\Program.cs:line 37

```
