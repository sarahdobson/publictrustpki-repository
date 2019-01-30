<ul class="usa-accordion">
  <li>
    <button class="usa-accordion-button"
      aria-expanded="false"
      aria-controls="c1">
      Where can I find copies of the Issuing and Root CA certificates?
    </button>
    <div id="c1" class="usa-accordion-content">
      Find copies of the Issuing and Root CA certificates below:
	  <br><br>
	  <strong>Issuing CA</strong>
	  <ul>
		<li>URL: <a href="{{ site.baseurl }}/assets/issuing.cert.cer" target="_blank">TBD</a></li>
		<li>SHA-256 Thumbprint: TBD</li>
		<li>Distinguished Name: TBD</li>
		<li>Serial Number: TBD</li>
		<li>Validity: TBD</li>
	  </ul>

	  <strong>Root CA</strong>	  
	  <ul>
		<li>URL: <a href="{{ site.baseurl }}/assets/root.cert.cer" target="_blank">TBD</a></li>
		<li>SHA-256 Thumbprint: TBD</li>
		<li>Distinguished Name: TBD</li>
		<li>Serial Number: TBD</li>
		<li>Validity: TBD</li>
	  </ul>
	  
	  <strong>Note:</strong> You should never install a root certificate without verifying it. Follow the examples below to verify the hash of the US Federal TLS Root CA certificate to ensure its integrity.
	  <br>
		<ul>
			<li>certutil -hashfile <i>filename.crt</i> SHA256</li>
			<li>openssl dgst -sha256 <i>filename.crt</i></li>
			<li>sha256sum <i>filename.crt</i></li>
		</ul>
		
    </div>
  </li>
  <li>
    <button class="usa-accordion-button"
      aria-expanded="false"
      aria-controls="c2">
      What kind of certificates does the PKI issue?
    </button>
    <div id="c2" class="usa-accordion-content">
	  The U.S. Federal Public Trust TLS PKI issues Domain-Validated (DV), RSA-2048 with SHA-256 TLS certificates. These certificates are compliant with the CA Browser Forum's <a href="https://cabforum.org/baseline-requirements" target="_blank">Baseline Requirements</a>.
	  <br><br>
	  Certificate request validation and issuance processes are automated through the use of the Automated Certificate Management Environment (ACME) protocol.
	</div>
  </li>
  <li>
    <button class="usa-accordion-button"
      aria-expanded="false"
      aria-controls="c3">
      Are certificates from the U.S. Federal Public Trust TLS PKI trusted by my browser?
    </button>
    <div id="c3" class="usa-accordion-content">
      Not yet.
	  <br><br>
	  We will be applying for inclusion into the following Trust Store Programs:
		<ul>
			<li>Microsoft Trust Store Program</li>
			<li>Apple Trust Store Program</li>
			<li>Mozilla Community and Trust Store Program</li>
			<li>Google Chromium</li>
		</ul>
    </div>
  </li>
  <li>
    <button class="usa-accordion-button"
      aria-expanded="false"
      aria-controls="c4">
      What is the lifetime for U.S. Federal Public Trust TLS PKI certificates? For how long are they valid?
    </button>
    <div id="c4" class="usa-accordion-content">
      Certificates will be valid for 13 months; however, we recommend that you automatically renew your certificates every 12 months. 
    </div>
  </li>
  <li>
    <button class="usa-accordion-button"
      aria-expanded="false"
      aria-controls="c5">
      Does the U.S. Federal Public Trust TLS PKI generate or store the private keys for my certificates on its servers?
    </button>
    <div id="c5" class="usa-accordion-content">
      No, never.  The private keys are always generated and managed on your server.
    </div>
  </li>  
</ul>
 


