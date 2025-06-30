1. [Vendor Info](#vendor-info)
   * [ADD_VENDOR_INFO](#add_vendor_info)
   * [UPDATE_VENDOR_INFO](#update_vendor_info)
   * [GET_VENDOR_INFO](#get_vendor_info)
   * [GET_ALL_VENDOR_INFO](#get_all_vendor_info)
2. [Model and Model Version](#model_and_model_version)
   * [ADD_MODEL](#add_model)
   * [EDIT_MODEL](#edit_model)
   * [DELETE_MODEL](#delete_model)
   * [ADD_MODEL_VERSION](#add_model_version)
   * [EDIT_MODEL_VERSION](#edit_model_version)
   * [DELETE_MODEL_VERSION](#delete_model_version)
   * [GET_MODEL](#get_model)
   * [GET_MODEL_VERSION](#get_model_version)
   * [GET_ALL_MODELS](#get_all_models)
   * [GET_ALL_VENDOR_MODELS](#get_all_vendor_models)
   * [GET_ALL_MODEL_VERSIONS](#get_all_model_versions)
3. [Compliance](#compliance)
   * [CERTIFY_MODEL](#certify_model)
   * [UPDATE_COMPLIANCE_INFO](#update_complince_info)
   * [DELETE_COMPLIANCE_INFO](#delete_complince_info)
   * [REVOKE_MODEL_CERTIFICATION](#revoke_model_certification)
   * [PROVISION_MODEL](#provision_model)
   * [GET_CERTIFIED_MODEL](#get_certified_model)
   * [GET_REVOKED_MODEL](#get_revoked_model)
   * [GET_PROVISIONAL_MODEL](#get_provisional_model)
   * [GET_COMPLIANCE_INFO](#get_compliance_info)
   * [GET_DEVICE_SOFTWARE_COMPLIANCE](#get_device_software_compliance)
   * [GET_ALL_CERTIFIED_MODELS](#get_all_certified_models)
   * [GET_ALL_REVOKED_MODELS](#get_all_revoked_models)
   * [GET_ALL_PROVISIONAL_MODELS](#get_all_provisional_models)
   * [GET_ALL_COMPLIANCE_INFO_RECORDS](#get_all_compliance_info_records)
   * [GET_ALL_DEVICE_SOFTWARE_COMPLIANCES](#get_all_device_software_compliances)
4. [X509 PKI](#X509-PKI)
   * [All Certificates (DA, NOC)](#all_certificates)
      * [GET_CERT](#get_cert)
      * [GET_ALL_CERTS](#get_all_certs)
      * [GET_ALL_CERTS_BY_SUBJECT](#get_all_certs_by_subjects)
      * [GET_ALL_CERTS_BY_SKID](#get_all_certs_by_skid)
      * [GET_CHILD_CERTS](#get_child_certs)
   * [Device Attestation Certificates](#device_attestation_certificate)
      * [PROPOSE_ADD_PAA](#propose_add_paa)
      * [APPROVE_ADD_PAA](#approve_add_paa)
      * [REJECT_ADD_PAA](#reject_add_paa)
      * [PROPOSE_REVOKE_PAA](#propose_revoke_paa)
      * [APPROVE_REVOKE_PAA](#approve_revoke_paa)
      * [ASSIGN_VID_TO_PAA](#assign_vid_to_paa)
      * [ADD_REVOCATION_DISTRIBUTION_POINT](#add_revocation_distribution_point)
      * [UPDATE_REVOCATION_DISTRIBUTION_POINT](#update_revocation_distribution_point)
      * [DELETE_REVOCATION_DISTRIBUTION_POINT](#delete_revocation_distribution_point)
      * [ADD_PAI](#add_pai)
      * [REVOKE_PAI](#revoke_pai)
      * [REMOVE_PAI](#remove_pai)
      * [GET_DA_CERT](#get_da_cert)
      * [GET_REVOKED_DA_CERT](#get_revoked_da_cert)
      * [GET_DA_CERTS_BY_SKID](#get_da_certs_by_skid)
      * [GET_DA_CERTS_BY_SUBJECT](#get_da_certs_by_subject)
      * [GET_ALL_DA_CERTS](#get_all_da_certs)
      * [GET_ALL_REVOKED_DA_CERTS](#get_all_revoked_da_certs)
      * [GET_PKI_REVOCATION_DISTRIBUTION_POINT](#get_pki_revocation_distribution_point)
      * [GET_PKI_REVOCATION_DISTRIBUTION_POINTS_BY_SUBJECT_KEY_ID](#get_pki_revocation_distribution_points_by_subject_key_id)
      * [GET_ALL_PKI_REVOCATION_DISTRIBUTION_POINT](#get_all_pki_revocation_distribution_point)
      * [GET_PROPOSED_PAA](#get_proposed_paa)
      * [GET_REJECTED_PAA](#get_rejected_paa)
      * [GET_PROPOSED_PAA_TO_REVOKE](#get_proposed_paa_to_revoke)
      * [GET_ALL_PAA](#get_all_paa)
      * [GET_ALL_REVOKED_PAA](#get_all_revoked_paa)
      * [GET_ALL_PROPOSED_PAA](#get_all_proposed_paa)
      * [GET_ALL_REJECTED_PAA](#get_all_rejected_paa)
      * [](#)
      * [](#)
      * [](#)
      * [](#)
      * [](#)
      * [](#)
      * [](#)
      * [](#)
      * [](#)
5. [Auth](#auth)
6. [Validator Node](#validator-node)
7. [Upgrade](#upgrade)

## [Vendor Info](transactions/vendor-info.md)

### [ADD_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#add_vendor_info)

#### CLI command
CLI command: `dcld tx vendorinfo add-vendor --vid=<uint16> --vendorName=<string> --companyLegalName=<string> --companyPreferredName=<string> --vendorLandingPageURL=<string> --from=<account>`
Test cases:
* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * access is denied to execute the command
      * incorrect command syntax
* Сommand result
   * Positive:
      * ADD_VENDOR_INFO command completed successfully **⇒** adds a record about a Vendor
   * Negative:
      * ADD_VENDOR_INFO command failed **⇒** does not add a record about a Vendor
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor (vendor role does not match Vendor ID)
      * CertificationCenter
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID
   * vendorName (Vendor name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative 
         * empty value	
   * companyLegalName (Company Legal Name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative
        * empty value	
   * companyPreferredName (Company Preferred Name)	optional(string)
      * Positive:
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative            
         * length > MAX	
   * vendorLandingPageURL (Vendor Landing Page URL)	optional(string)
      * Positive:
         * value exists	
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative              
         * length > MAX	
         * сontains spaces or line breaks	
   * schemaVersion (Schema Version)	optional(uint16)
      * Positive:
         * value = 0	
         * integer value format	
         * empty value	
      * Negative 	
         * length > MAX	MAX = 65535
#### REST API 
POST: `/cosmos/tx/v1beta1/txs`[NewMsgCreateVendorInfo](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/proto/zigbeealliance/distributedcomplianceledger/vendorinfo/tx.proto#L18)
Test cases:
* REST API command send
   * Positive:
      * correct HTTP method
      * request is authorized
      * uses valid credentials/role
   * Negative:
      * incorrect request
      * server-side error
* Сommand result
   * Positive:
      * ADD_VENDOR_INFO command completed successfully **⇒** adds a record about a Vendor
   * Negative:
      * ADD_VENDOR_INFO command failed **⇒** does not add a record about a Vendor
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor (vendor role does not match Vendor ID)
      * CertificationCenter
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID
   * vendorName (Vendor name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative 
         * empty value	
   * companyLegalName (Company Legal Name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative
        * empty value	
   * companyPreferredName (Company Preferred Name) - optional(string)
      * Positive:
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative            
         * length > MAX	
   * vendorLandingPageURL (Vendor Landing Page URL) - optional(string)
      * Positive:
         * value exists	
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative              
         * length > MAX	
         * сontains spaces or line breaks	
   * schemaVersion (Schema Version) - optional(uint16)
      * Positive:
         * value = 0	
         * integer value format	
         * empty value	
      * Negative 	
         * length > MAX	MAX = 65535

### [UPDATE_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#update_vendor_info)
#### CLI command
CLI command: `dcld tx vendorinfo update-vendor --vid=<uint16> ... --from=<account>`
Test cases:
* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * access is denied to execute the command
      * incorrect command syntax
* Сommand result
   * Positive:
      * UPDATE_VENDOR_INFO command completed successfully **⇒** updates a record about a Vendor
         * ADD_VENDOR_INFO command completed successfully
         * There is at least one record about a Vendor
   * Negative:
      * UPDATE_VENDOR_INFO command failed **⇒** does not update a record about a Vendor
         * ADD_VENDOR_INFO command was not executed
         * There is no one record about a Vendor
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor (vendor role does not match Vendor ID)
      * CertificationCenter
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID
   * vendorName (Vendor name) - string 
      * Positive:	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * empty value	
   * companyLegalName (Company Legal Name) - string 
      * Positive:	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * empty value	
   * companyPreferredName (Company Preferred Name) - optional(string)
      * Positive:	
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * length > MAX	
   * vendorLandingPageURL (Vendor Landing Page URL) - optional(string)
      * Positive:	
         * value exists	
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * length > MAX	
         * сontains spaces or line breaks	
   * schemaVersion (Schema Version) - optional(uint16)
      * Positive:	
         * value = 0	
         * integer value format	
         * empty value	
      * Negative 	
         * length > MAX	MAX = 65535
#### REST API 
POST: `/cosmos/tx/v1beta1/txs`[MsgUpdateVendorInfo](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/proto/zigbeealliance/distributedcomplianceledger/vendorinfo/tx.proto#L30)
Test cases:
* REST API command send
   * Positive:
      * correct HTTP method
      * request is authorized
      * uses valid credentials/role
   * Negative:
      * incorrect request
      * server-side error
* Сommand result
   * Positive:
      * UPDATE_VENDOR_INFO command completed successfully **⇒** updates a record about a Vendor
         * ADD_VENDOR_INFO command completed successfully
         * There is at least one record about a Vendor
   * Negative:
      * UPDATE_VENDOR_INFO command failed **⇒** does not update a record about a Vendor
         * ADD_VENDOR_INFO command was not executed
         * There is no one record about a Vendor
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor (vendor role does not match Vendor ID)
      * CertificationCenter
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID
   * vendorName (Vendor name) - string 
      * Positive:	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * empty value	
   * companyLegalName (Company Legal Name) - string 
      * Positive:	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * empty value	
   * companyPreferredName (Company Preferred Name) - optional(string)
      * Positive:	
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * length > MAX	
   * vendorLandingPageURL (Vendor Landing Page URL) - optional(string)
      * Positive:	
         * value exists	
         * empty value	
         * text value format	
         * MIN < length < MAX	
      * Negative 	
         * length > MAX	
         * сontains spaces or line breaks	
   * schemaVersion (Schema Version) - optional(uint16)
      * Positive:	
         * value = 0	
         * integer value format	
         * empty value	
      * Negative 	
         * length > MAX	MAX = 65535
### [GET_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#get_vendor_info)
#### CLI command
CLI command: `dcld query vendorinfo vendor --vid=<uint16>`
Test cases:
* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * access is denied to execute the command
      * incorrect command syntax
* Сommand result
   * Positive:
      * GET_VENDOR_INFO command completed successfully **⇒** gets a Vendor Info for the given vid (vendor ID)
         * there is at least one Vendor Info for the given vid (vendor ID)
   * Negative:
      * GET_VENDOR_INFO command failed **⇒** does not gets a Vendor Info for the given vid (vendor ID)
         * there is not one Vendor Info for the given vid (vendor ID)
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor 
      * VendorAdmin 
      * CertificationCenter 
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID
#### REST API 
GET: `/dcl/vendorinfo/vendors/{vid}`
Test cases:
* REST API command send
   * Positive:
      * correct HTTP method
      * request is authorized
      * uses valid credentials/role
   * Negative:
      * incorrect request
      * server side error
* Сommand result
   * Positive:
      * GET_VENDOR_INFO command completed successfully **⇒** gets a Vendor Info for the given vid (vendor ID)
         * there is at least one Vendor Info for the given vid (vendor ID)
   * Negative:
      * GET_VENDOR_INFO command failed **⇒** does not gets a Vendor Info for the given vid (vendor ID)
         * there is not one Vendor Info for the given vid (vendor ID)
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor 
      * VendorAdmin 
      * CertificationCenter 
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID
### [GET_ALL_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#get_all_vendor_info)
#### CLI command
CLI command: `dcld query vendorinfo all-vendors`
Test cases:
* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * access is denied to execute the command
      * incorrect command syntax
* Сommand result
   * Positive:
      * GET_ALL_VENDOR_INFO command completed successfully **⇒** gets information about all vendors for all VIDs
         * there is at least one Vendor for all VIDs
   * Negative:
      * GET_ALL_VENDOR_INFO command failed **⇒** does not information about all vendors for all VIDs
         * there is not one  Vendor for all VIDs
* Role (Who can send)
   * Positive:
      * Trustee
      * Vendor 
      * VendorAdmin 
      * CertificationCenter 
      * NodeAdmin 
* Parameters:
   * count-total - optional(bool)
      * Positive:
         * empty value
         * value state
            * TRUE (-1)
            * FALSE (0)
      * Negative 
         * value is not bool
   * limit - optional(uint)
      * Positive:	
         * value exists	
         * empty value	
      * Negative	
         * value > 100	
   * offset - optional(uint)
      * Positive:	
         * value exists	
         * empty value	
      * Negative	
         * value < 0	
   * page - optional(uint)
      * Positive:	
         * value exists	
         * empty value	
      * Negative	
         * value < 0	
   * page-key - optional(string)
      * Positive:	
         * empty value	
         * value exists	
      * Negative	
         * length < MIN	
   * reverse - optional(bool)
      * Positive:	
         * empty value	
         * value state	
            * TRUE (-1)	
            * FALSE (0)	
      * Negative	
         * value is not bool	
#### REST API 
GET: `/dcl/vendorinfo/vendors`
Test cases:
* REST API command send
   * Positive:
      * correct HTTP method
      * request is authorized
      * uses valid credentials/role
   * Negative:
      * incorrect request
      * server side error
* Сommand result
   * Positive:
      * GET_ALL_VENDOR_INFO command completed successfully **⇒** gets information about all vendors for all VIDs
         * there is at least one Vendor for all VIDs
   * Negative:
      * GET_ALL_VENDOR_INFO command failed **⇒** does not information about all vendors for all VIDs
         * there is not one  Vendor for all VIDs
* Role (Who can send)
   * Positive:
      * Trustee
      * Vendor 
      * VendorAdmin 
      * CertificationCenter 
      * NodeAdmin 
* Parameters:
   * count-total - optional(bool)
      * Positive:
         * empty value
         * value state
            * TRUE (-1)
            * FALSE (0)
      * Negative 
         * value is not bool
   * limit - optional(uint)
      * Positive:	
         * value exists	
         * empty value	
      * Negative	
         * value > 100	
   * offset - optional(uint)
      * Positive:	
         * value exists	
         * empty value	
      * Negative	
         * value < 0	
   * page - optional(uint)
      * Positive:	
         * value exists	
         * empty value	
      * Negative	
         * value < 0	
   * page-key - optional(string)
      * Positive:	
         * empty value	
         * value exists	
      * Negative	
         * length < MIN	
   * reverse - optional(bool)
      * Positive:	
         * empty value	
         * value state	
            * TRUE (-1)	
            * FALSE (0)	
      * Negative	
         * value is not bool	

## Vendor Info
### [ADD_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#add_vendor_info)
#### CLI command
CLI command: `dcld tx vendorinfo add-vendor --vid=<uint16> --vendorName=<string> --companyLegalName=<string> --companyPreferredName=<string> --vendorLandingPageURL=<string> --from=<account>`
Test cases:
* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * access is denied to execute the command
      * incorrect command syntax
* Сommand result
   * Positive:
      * ADD_VENDOR_INFO command completed successfully **⇒** adds a record about a Vendor
   * Negative:
      * ADD_VENDOR_INFO command failed **⇒** does not add a record about a Vendor
* Role (Who can send)
   * Positive:
      * Vendor (vendor role the matching Vendor ID)
      * VendorAdmin 
   * Negative:
      * Trustee
      * Vendor (vendor role does not match Vendor ID)
      * CertificationCenter
      * NodeAdmin 
* Parameters:
   * vid (Vendor ID) - uint16:
      * Positive:
         * value exists
         * value > 0
         * integer value format
      * Negative 
         * empty value
         * length > MAX (MAX = 65535)
         * nonexistent ID


## Add DA Root

### [Propose adding of DA root certificate](./handler_propose_paa_cert_test.go)

Indexes to check:

* Present:
    * `ProposedCertificate`
    * `UniqueCertificate`
* Missing:
    * `RejectedCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), Subject+SKID (root), SKID, Subject

Test cases:

* Positive:
    * Propose single certificate: `TestHandler_ProposeAddDaRootCert`
    * Propose two certificates with same SKID but different Subject:
      `TestHandler_ProposeAddDaRootCert_SameSkidButDifferentSubject`
    * Propose certificate with Subject/SKID same as existing Approved certificate, but different SerialNumber:
      `TestHandler_ProposeAddDaRootCert_DifferentSerialNumber`
    * Propose adding of previously rejected certificate: `TestHandler_ProposeAddDaRootCert_PreviouslyRejected`
* Negative:
    * Propose by not Trustee: `TestHandler_ProposeAddDaRootCert_ByNotTrustee`
    * Propose invalid certificate: `TestHandler_ProposeAddDaRootCert_ForInvalidCertificate`
    * Propose with existing proposed certificate (Subject/SKID): `TestHandler_ProposeAddDaRootCert_Duplicate`
    * Propose with existing approved certificate (Subject/SKID/SerialNumber):
      `TestHandler_ProposeAddDaRootCert_CertificateAlreadyExists`
    * Propose not self-signed certificate: `TestHandler_ProposeAddDaRootCert_ForNonRootCertificate`
    * Propose not root certificate: `TestHandler_ProposeAddDaRootCert_ForNonRootCertificate`
    * Propose NOC root certificate: can we check it? `TestHandler_ProposeAddDaRootCert_ForNocCertificate` - wrong test.
    * Propose with existing approved subject/SKID where signer is not owner of active:
      `TestHandler_ProposeAddDaRootCert_ForDifferentSigner`

### [Approve adding of DA root certificate](handler_approve_add_paa_cert_test.go)

Indexes:

* Present:
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), Subject+SKID (root), SKID, Subject
* Missing:
    * `ProposedCertificate`

Test cases:

* Positive:
    * Approve certificate for not enough approvals: `TestHandler_AddDaRootCert_TwoThirdApprovalsNeeded`
  * Add certificate: `TestHandler_AddDaRootCert`,
    `TestHandler_AddDaRootCert_TwoThirdApprovalsNeeded`,
    `TestHandler_AddDaRootCert_FourOfFiveApprovalsAreNeeded`
  * Add two certificates with same SKID but different Subject:
    `TestHandler_AddDaRootCert_SameSkid_DifferentSubject`
  * Add two certificates with same Subject but different SKID:
  * Add two certificates with same Subject and SKID:
    `TestHandler_AddDaRootCert_SameSubjectAndSkid_DifferentSerialNumber`
  * Approve certificate which was previously rejected by the current user:
    `TestHandler_ApproveAddDaRootCert_PreviouslyRejectedByCurrentTrustee`
* Negative:
    * Approve by not Trustee: `TestHandler_ApproveAddDaRootCert_ByNotTrustee`
    * Approve of non-existing proposed certificate: `TestHandler_ApproveAddDaRootCert_UnknownProposedCertificate`
    * Approve certificate already approved by the current user: `TestHandler_ApproveAddDaRootCert_Twice`

### [Reject adding of DA root certificate](handler_reject_add_paa_cert_test.go)

Indexes:

* Present:
    * `RejectedCertificate`
* Missing:
    * `ProposedCertificate`
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), Subject+SKID (root), SKID, Subject

Test cases:

* Positive:
    * Propose add reject adding of DA root certificate: `TestHandler_RejectAddDaRootCert`,
      `TestHandler_RejectX509RootCert_TwoRejectApprovalsAreNeeded_FiveTrustees`
    * Reject adding of DA root certificate for not enough rejects: `TestHandler_RejectAddDaRootCert`,
      `TestHandler_RejectX509RootCert_TwoRejectApprovalsAreNeeded_FiveTrustees`
    * Reject DA root certificate - certificate still has other approval (certificates must be proposed):
      `TestHandler_RejectAddDaRootCert_CertificateHasOtherApproval`
    * Reject DA root certificate - certificate still has other reject (certificates must be proposed):
      `TestHandler_RejectAddDaRootCert_CertificateHasOtherReject`
    * Reject DA root certificate - certificate does not have other rejects/approvals (certificates must be removed):
      `TestHandler_RejectAddDaRootCert_CertificateNotHasOtherApprovalAndRejects`
* Negative:
    * Reject by not Trustee: `TestHandler_RejectAddDaRootCert_ByNotTrustee`
    * Reject of non-existing proposed certificate: `TestHandler_RejectAddDaRootCert_UnknownProposedCertificate`
    * Reject certificate already rejected by the current user: `TestHandler_RejectAddDaRootCert_Twice`

## [Add DA Intermediate](./handler_add_pai_cert_test.go)

Indexes to check:

* Present:
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), SKID, Subject
    * `ChildCertificates`: for parent
* Missing:
    * `ProposedCertificate`

Test cases:

* Positive:
    * Add intermediate certificate: `TestHandler_AddDaIntermediateCert`,
      `TestHandler_AddDaIntermediateCert_VidScoped`
    * Add two certificates with same Subject/SKID but different SerialNumber:
      `TestHandler_AddDaIntermediateCert_SameSubjectAndSkid_DifferentSerialNumber`
    * Add two certificates with same Subject but different SKID: ?
    * Add two certificates with same SKID but different Subject: ?
    * Add tree of certificates (root, intermediate, leaf): `TestHandler_AddDaIntermediateCert_ForTree`
    * Add intermediate certificate but other Vendor with the same VID:
      `TestHandler_AddDaIntermediateCert_ByNotOwnerButSameVendor`
* Negative:
    * Add by not Vendor: `TestHandler_AddDaIntermediateCert_SenderNotVendor`
    * Add invalid certificate: `TestHandler_AddDaIntermediateCert_ForInvalidCertificate`
    * Add self-signed certificate: `TestHandler_AddDaIntermediateCert_ForRootCertificate`
    * Add with existing issuer/serial number: `TestHandler_AddDaIntermediateCert_ForDuplicate`
    * Add for root certificate: `TestHandler_AddDaIntermediateCert_ForRootCertificate`
    * Add for root NOC certificate: `TestHandler_AddDaIntermediateCert_RootIsNoc`
    * Add NOC certificate: TBD
    * Add with different VID: `TestHandler_AddDaIntermediateCert_ByOtherVendor`
    * Add with invalid chain: `TestHandler_AddDaIntermediateCert_ForAbsentDirectParentCert`

## Revoke DA Root

### [Propose revocation of DA root certificate](handler_propose_revoke_paa_cert_test.go)

Indexes to check:

* Present:
    * `ProposedCertificateRevocation`
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), Subject+SKID (root), SKID, Subject
* Missing:
    * `RevokedCertificates`
    * `RevokedRootCertificates`

Test cases:

* Positive:
    * Propose revocation by Subject/SKID/SerialNumber - single certificate: `TestHandler_ProposeRevokeDaRootCert`
    * Propose revocation by Subject/SKID/SerialNumber - two certificates:
      `TestHandler_ProposeRevokeDaRootCert_TwoCertificates`
    * Propose revocation by Subject/SKID/SerialNumber - revoke child: `TestHandler_ProposeRevokeDaRootCert_RevokeChild`
    * Propose revocation by Subject/SKID/SerialNumber - keep child: `TestHandler_ProposeRevokeDaRootCert_KeepChild`
    * Propose revocation by other Vendor with the same VID: `TestHandler_ProposeRevokeDaRootCert_ByTrusteeNotOwner`
* Negative:
    * Propose revocation by not Trustee: `TestHandler_ProposeRevokeDaRootCert_ByNotTrustee`
    * Propose revocation of already proposed for revocation:
      `TestHandler_ProposeRevokeDaRootCert_ProposedRevocationAlreadyExists`
    * Propose revocation of not existing approved certificate (Subject/SKID):
      `TestHandler_ProposeRevokeDaRootCert_CertificateDoesNotExist`,
      `TestHandler_ProposeRevokeDaRootCert_ForProposedCertificate`
    * Propose revocation of not existing approved certificate (Subject/SKID + SerialNumber):
      `TestHandler_ProposeRevokeDaRootCert_CertificateDoesNotExistBySerialNumber`
    * Propose revocation of not root certificate: `TestHandler_ProposeRevokeDaRootCert_ForNonRootCertificate`

### [Approve revocation of DA root certificate](handler_approve_revoke_paa_cert_test.go)

Indexes:

* Present:
    * `RevokedCertificates`
    * `RevokedRootCertificates`
    * `UniqueCertificate`
* Missing:
    * `ProposedCertificateRevocation`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), Subject+SKID (root), SKID, Subject

Test cases:

* Positive:
    * Approve revocation DA root certificate when not enough approvals:
      `TestHandler_ApproveRevokeDaRootCert_NotEnoughApprovals`
    * Revoke by Subject/SKID: `TestHandler_RevokeDaRootCert_BySubjectAndSKID`,
      `TestHandler_RevokeDaRootCert_TwoThirdApprovalsNeeded`
    * Revoke by Subject/SKID/SerialNumber: `TestHandler_RevokeDaRootCert_BySerialNumber`
    * Revoke by Subject/SKID/SerialNumber - revoke child: `TestHandler_RevokeDaRootCert_RevokeChild`
    * Revoke by Subject/SKID/SerialNumber - keep child: `TestHandler_RevokeDaRootCert_KeepChild`
    * Revoke by Subject/SKID when two certs with the same SKID exist:
      `TestHandler_RevokeDaRootCert_BySubjectAndSkid_TwoCertificatesWithSameSkid`
    * Revoke by Subject/SKID when two certs with the same Subject exist: ?
* Negative:
    * Approve revocation by not Trustee: `TestHandler_ApproveRevokeDaRootCert_ByNotTrustee`
    * Approve revocation of not existing certificate (Subject/SKID):
      `TestHandler_ApproveRevokeDaRootCert_ProposedRevocationDoesNotExist`
    * Approve certificate revocation by not existing serial number (Subject/SKID + SerialNumber):
      `TestHandler_ApproveRevokeDaRootCert_BySerialNumber_ProposedRevocationDoesNotExist`
    * Approve certificate revocation twice by the same user: `TestHandler_ApproveRevokeDaRootCert_Twice`

## [Revoke DA Intermediate](./handler_revoke_pai_cert_test.go)

Indexes to check:

* Present:
    * `RevokedCertificates`
    * `UniqueCertificate`
    * Root - stays approved
* Missing:
    * `ProposedCertificateRevocation`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), SKID, Subject
    * `ChildCertificates`: for parent

Test cases:

* Positive:
    * Revoke by Subject/SKID: `TestHandler_RevokeDaIntermediateCert_BySubjectAndSKID`
    * Revoke by Subject/SKID/SerialNumber: `TestHandler_RevokeDaIntermediateCert_BySerialNumber`
    * Revoke by Subject/SKID - revoke child: `TestHandler_RevokeDaIntermediateCert_BySubjectAndSKID_RevokeChild`
    * Revoke by Subject/SKID/SerialNumber - revoke child:
      `TestHandler_RevokeDaIntermediateCert_BySerialNumber_RevokeChild`
    * Revoke by Subject/SKID - keep child: `TestHandler_RevokeDaIntermediateCert_BySubjectAndSKID_KeepChild`
    * Revoke by Subject/SKID/SerialNumber - keep child: `TestHandler_RevokeDaIntermediateCert_BySerialNumber_KeepChild`
    * Revoke by Subject/SKID - parent not affected: `TestHandler_RevokeDaIntermediateCert_BySubjectAndSKID_ParentExist`
    * Revoke by Subject/SKID/SerialNumber - parent not affected:
      `TestHandler_RevokeDaIntermediateCert_BySerialNumber_ParentExist`
    * Revoke by Subject/SKID - another certificate with same Subject exist: ?
    * Revoke by Subject/SKID - another certificate with same SKID exist: ?
    * Revoke by other Vendor with the same VID: `TestHandler_RevokeDaIntermediateCert_ByNotOwnerButSameVendor`
* Negative:
    * Revoke by not Vendor: `TestHandler_RevokeDaIntermediateCert_SenderNotVendor`
    * Revoke root certificate: `TestHandler_RevokeDaIntermediateCert_ForRootCertificate`
    * Revoke by Vendor with different VID: `TestHandler_RevokeDaIntermediateCert_ByVendorWithOtherVid`
    * Revoke not existing certificate (Subject/SKID): `TestHandler_RevokeDaIntermediateCert_CertificateDoesNotExist`
    * Revoke not existing certificate by SerialNumber (Subject/SKID + SerialNumber):
      `TestHandler_RevokeDaIntermediateCert_CertificateDoesNotExistBySerialNumber`

## [Remove DA Intermediate](./handler_remove_pai_cert_test.go)

Indexes to check:

* Present:
    * no
* Missing:
    * `RevokedCertificates`
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `DA Certificates`: Subject+SKID (approved), SKID, Subject
    * `ChildCertificates`: for parent

Test cases:

* Positive:
    * Remove by Subject/SKID: `TestHandler_RemoveDaIntermediateCert_BySubjectAndSKID`
    * Remove by Subject/SKID/SerialNumber: `TestHandler_RemoveDaIntermediateCert_BySerialNumber`
    * Remove by Subject/SKID - parent exist: `TestHandler_RemoveDaIntermediateCert_BySubjectAndSKID_ParentExist`
    * Remove by Subject/SKID/SerialNumber - parent exist:
      `TestHandler_RemoveDaIntermediateCert_BySerialNumber_ParentExist`
    * Remove by Subject/SKID - approved child exist:
      `TestHandler_RemoveDaIntermediateCert_BySubjectAndSKID_ApprovedChildExist`
    * Remove by Subject/SKID/SerialNumber - approved child exist:
      `TestHandler_RemoveDaIntermediateCert_BySerialNumber_ApprovedChildExist`
    * Remove by Subject/SKID - approved child exist:
      `TestHandler_RemoveDaIntermediateCert_BySubjectAndSKID_RevokedChildExist`
    * Remove by Subject/SKID/SerialNumber - approved child exist:
      `TestHandler_RemoveDaIntermediateCert_BySerialNumber_RevokedChildExist`
    * Remove by Subject/SKID - revoked certificate:
      `TestHandler_RemoveDaIntermediateCert_BySubjectAndSKID_RevokedCertificate`
    * Remove by Subject/SKID/SerialNumber - revoked certificate:
      `TestHandler_RemoveDaIntermediateCert_BySerialNumber_RevokedCertificate`
    * Remove by Subject/SKID - revoked and active certificates:
      `TestHandler_RemoveDaIntermediateCert_BySubjectAndSKID_RevokedAndActiveCertificate`
    * Remove by Subject/SKID - another certificate with same Subject exist: ?
    * Remove by Subject/SKID - another certificate with same SKID exist: ?
    * Remove by other Vendor with the same VID: `TestHandler_RemoveDaIntermediateCert_ByNotOwnerButSameVendor`
* Negative:
    * Remove by not Vendor: `TestHandler_RemoveDaIntermediateCert_SenderNotVendor`
    * Remove not existing certificated (Subject/SKID): `TestHandler_RemoveDaIntermediateCert_CertificateDoesNotExist`
    * Remove not existing certificated (Subject/SKID + SerialNumber):
      `TestHandler_RemoveDaIntermediateCert_InvalidSerialNumber`
    * Remove root certificate: `TestHandler_RemoveDaIntermediateCert_ForRootCertificate`
    * Remove NOC certificate: `TestHandler_RemoveDaIntermediateCert_ForNocIcaCertificate`
    * Remove by other Vendor with different VID: `TestHandler_RemoveDaIntermediateCert_ByOtherVendor`

## [Add Noc Root](./handler_add_noc_root_cert_test.go)

Indexes to check:

* Present:
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `Noc Certificates`: Subject+SKID, SKID, Subject, VID (root), VID+SKID
* Missing:
    * no

Test cases:

* Positive:
    * Add certificate: `TestHandler_AddNocRootCert`
    * Add two certificates with same Subject/SKID but different SerialNumber:
      `TestHandler_AddNocRootCert_SameSubjectAndSkid_DifferentSerialNumber`
    * Add certificates with same Subject but different SKID: ?
    * Add two certificates with same SKID but different Subject: ?
    * Add two certificates but different Vendors with same VID: `TestHandler_AddNocRootCert_ByNotOwnerButSameVendor`
* Negative:
    * Add by not Vendor: `TestHandler_AddNocRootCert_SenderNotVendor`
    * Add invalid certificate: `TestHandler_AddNocRootCert_InvalidCertificate:NotValidPemCertificate`
    * Add not root: `TestHandler_AddNocRootCert_InvalidCertificate:NonRootCertificate`
    * Add with existing Issuer/SerialNumber: `TestHandler_AddNocRootCert_CertificateExist:Duplicate`
    * Add DA certificate: `TestHandler_AddNocRootCert_CertificateExist:ExistingNotNocCert`
    * Add by Vendor with different VID: `TestHandler_AddNocRootCert_CertificateExist:ExistingCertWithDifferentVid`

## [Add Noc Intermediate](./handler_add_noc_ica_cert_test.go)

Indexes to check:

* Present:
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `Noc Certificates`: Subject+SKID, SKID, Subject, VID (ica), VID+SKID
    * `ChildCertificates`: for parent
* Missing:
    * no

Test cases:

* Positive:
    * Add certificate: `TestHandler_AddNocIntermediateCert`
    * Add two certificates with same Subject/SKID but different SerialNumber:
      `TestHandler_AddNocIntermediateCert_SameSubjectAndSkid_DifferentSerialNumber`
    * Add two certificates with same Subject but different SKID: ?
    * Add two certificates with same SKID but different Subject: ?
    * Add two certificates but different Vendors with same VID:
      `TestHandler_AddNocIntermediateCert_ByNotOwnerButSameVendor`
* Negative:
    * Add by not Vendor: `TestHandler_AddNocIntermediateCert_SenderNotVendor`
    * Add invalid certificate: `TestHandler_AddNocIntermediateCert_ForInvalidCertificate`
    * Add NOC root: `TestHandler_AddNocIntermediateCert_ForNocRootCertificate`
    * Add with existing Issuer/SerialNumber: `TestHandler_AddNocIntermediateCert_CertificateExist`
    * Add for invalid chain of parent certificates: `TestHandler_AddNocIntermediateCert_WhenNocRootCertIsAbsent`
    * Add DA certificate: `TestHandler_AddNocIntermediateCert_ForRootNonNocCertificate`
    * Add by Vendor with different VID: `TestHandler_AddNocIntermediateCert_Root_VID_Does_Not_Equal_To_AccountVID`

## [Revoke Noc Root](./handler_revoke_noc_root_cert_test.go)

Indexes:

* Present:
    * `RevokedCertificates` (root)
    * `UniqueCertificate`
* Missing:
    * `RevokedCertificates` (ica)
    * `All Certificates`: Subject+SKID, SKID, Subject
        * `Noc Certificates`: Subject+SKID, SKID, Subject, VID (root), VID+SKID

* Positive:
    * Revoke by Subject/SKID: `TestHandler_RevokeNocRootCert_BySubjectAndSKID`
    * Revoke by Subject/SKID/SerialNumber: `TestHandler_RevokeNocRootCert_BySerialNumber`
    * Revoke by Subject/SKID - revoke child: `TestHandler_RevokeNocRootCert_BySubjectAndSKID_RevokeChild`
    * Revoke by Subject/SKID/SerialNumber - revoke child: `TestHandler_RevokeNocRootCert_BySerialNumber_RevokeChild`
    * Revoke by Subject/SKID - keep child: `TestHandler_RevokeNocRootCert_BySubjectAndSKID_KeepChild`
    * Revoke by Subject/SKID/SerialNumber - keep child: `TestHandler_RevokeNocRootCert_BySerialNumber_KeepChild`
    * Revoke by Subject/SKID - another certificate with same Subject exist: ?
    * Revoke by Subject/SKID - another certificate with same SKID exist: ?
    * Revoke by other Vendor with the same VID: `TestHandler_RevokeNocRootCert_OtherVendor`
* Negative:
    * Revoke by not Vendor: `TestHandler_RevokeNocRootCert_SenderNotVendor`
    * Revoke not existing certificate (Subject/SKID): `TestHandler_RevokeNocRootCert_CertificateDoesNotExist`
    * Revoke not existing certificate by SerialNumber (Subject/SKID + SerialNumber):
      `TestHandler_RevokeNocRootCert_CertificateExists`
    * Revoke not root certificate: `TestHandler_RevokeNocRootCert_CertificateExists`
    * Revoke not NOC certificate: `TestHandler_RevokeNocRootCert_CertificateExists`
    * Revoke by Vendor with different VID: `TestHandler_RevokeNocRootCert_CertificateExists`

## [Revoke Noc Ica](./handler_revoke_noc_ica_cert_test.go)

Indexes:

* Present:
    * `RevokedCertificates` (ica)
    * `UniqueCertificate`
* Missing:
    * `RevokedCertificates` (root)
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `Noc Certificates`: Subject+SKID, SKID, Subject, VID (ica), VID+SKID
    * `ChildCertificates`: for parent

Test cases:

* Positive:
    * Revoke by Subject/SKID: `TestHandler_RevokeNocIntermediateCert_BySubjectAndSKID`
    * Revoke by Subject/SKID/SerialNumber: `TestHandler_RevokeNocIntermediateCert_BySerialNumber`
    * Revoke by Subject/SKID - revoke child: `TestHandler_RevokeNocIntermediateCert_BySubjectAndSKID_RevokeChild`
    * Revoke by Subject/SKID/SerialNumber - revoke child:
      `TestHandler_RevokeNocIntermediateCert_BySerialNumber_RevokehChild`
    * Revoke by Subject/SKID - keep child: `TestHandler_RevokeNocIntermediateCert_BySubjectAndSKID_KeepChild`
    * Revoke by Subject/SKID/SerialNumber - keep child: `TestHandler_RevokeNocIntermediateCert_BySerialNumber_KeepChild`
    * Revoke by Subject/SKID - parent not affected: `TestHandler_RevokeNocIntermediateCert_BySubjectAndSKID_ParentExist`
    * Revoke by Subject/SKID/SerialNumber - parent not affected:
      `TestHandler_RevokeNocIntermediateCert_BySerialNumber_ParentExist`
    * Revoke by Subject/SKID - another certificate with same Subject exist: ?
    * Revoke by Subject/SKID - another certificate with same SKID exist: ?
    * Revoke by other Vendor with the same VID: `TestHandler_RevokeNocIntermediateCert_ByOtherVendor`
* Negative:
    * Revoke by not Vendor: `TestHandler_RevokeNocIntermediateCert_SenderNotVendor`
    * Revoke not existing certificate by Subject/SKID: `TestHandler_RevokeNocIntermediateCert_CertificateDoesNotExist`
    * Revoke not existing certificate by Subject/SKID/SerialNumber:
      `TestHandler_RevokeNocIntermediateCert_CertificateExists`
    * Revoke root certificate: `TestHandler_RevokeNocIntermediateCert_CertificateExists`
    * Revoke root DA certificate: `TestHandler_RevokeNocIntermediateCert_CertificateExists`
    * Revoke by Vendor with different VID: `TestHandler_RevokeNocIntermediateCert_CertificateExists`

## [Remove Noc Root](./handler_remove_noc_root_cert_test.go)

Indexes to check:

* Present:
    * no
* Missing:
    * `RevokedCertificates` (root)
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `Noc Certificates`: Subject+SKID, SKID, Subject, VID (root), VID+SKID

Test cases:

* Positive:
    * Remove by Subject/SKID: `TestHandler_RemoveNocRootCert_BySubjectAndSKID`
    * Remove by Subject/SKID/SerialNumber: `TestHandler_RemoveNocRootCert_BySerialNumber`
    * Remove by Subject/SKID - child exist: `TestHandler_RemoveNocRootCert_BySubjectAndSKID_ChildExist`
    * Remove by Subject/SKID/SerialNumber - child exist: `TestHandler_RemoveNocRootCert_BySerialNumber_ChildExist`
    * Remove by Subject/SKID - revoked certificate:
      `TestHandler_RemoveNocRootCert_BySubjectAndSKID_RevokedCertificate`
    * Remove by Subject/SKID/SerialNumber - revoked certificate:
      `TestHandler_RemoveNocRootCert_BySerialNumber_RevokedCertificate`
    * Remove by Subject/SKID - revoked and active certificates:
      `TestHandler_RemoveNocRootCert_BySubjectAndSKID_RevokedAndActiveCertificate`
    * Remove by Subject/SKID - another certificate with same Subject exist: ?
    * Remove by Subject/SKID - another certificate with same SKID exist: ?
    * Remove by other Vendor with the same VID: `TestHandler_RemoveNocRootCert_ByNotOwnerButSameVendor`
* Negative:
    * Remove by not Vendor: `TestHandler_RemoveNocRootCert_SenderNotVendor`
    * Remove not existing certificated (Subject/SKID): `TestHandler_RemoveNocRootCert_CertificateDoesNotExist`
    * Remove not existing certificated (Subject/SKID + SerialNumber):
      `TestHandler_RemoveNocRootCert_InvalidSerialNumber`
    * Remove intermediate certificate: `TestHandler_RemoveNocRootCert_IntermediateCertificate`
    * Remove DA certificate: `TestHandler_RemoveNocRootCert_DaCertificate`
    * Remove by other Vendor with different VID: `TestHandler_RemoveNocRootCert_ByOtherVendor`

## [Remove Noc Intermediate](./handler_remove_noc_ica_cert_test.go)

Indexes to check:

* Present:
    * no
* Missing:
    * `RevokedCertificates` (ica)
    * `UniqueCertificate`
    * `All Certificates`: Subject+SKID, SKID, Subject
    * `Noc Certificates`: Subject+SKID, SKID, Subject, VID (ica), VID+SKID
    * `ChildCertificates`: for parent

Test cases:

* Positive:
    * Remove by Subject/SKID: `TestHandler_RemoveNocIntermediateCert_BySubjectAndSKID`
    * Remove by Subject/SKID/SerialNumber: `TestHandler_RemoveNocIntermediateCert_BySerialNumber`
    * Remove by Subject/SKID - parent exist: `TestHandler_RemoveNocIntermediateCert_BySubjectAndSKID_ParentExist`
    * Remove by Subject/SKID/SerialNumber - parent exist:
      `TestHandler_RemoveNocIntermediateCert_BySerialNumber_ParentExist`
    * Remove by Subject/SKID - approved child exist:
      `TestHandler_RemoveNocIntermediateCert_BySubjectAndSKID_ApprovedChildExist`
    * Remove by Subject/SKID/SerialNumber - approved child exist:
      `TestHandler_RemoveNocIntermediateCert_BySerialNumber_ApprovedChildExist`
    * Remove by Subject/SKID - revoked child exist:
      `TestHandler_RemoveNocIntermediateCert_BySubjectAndSKID_RevokedChildExist`
    * Remove by Subject/SKID/SerialNumber - revoked child exist:
      `TestHandler_RemoveNocIntermediateCert_BySerialNumber_RevokedChildExist`
    * Remove by Subject/SKID - revoked certificate:
      `TestHandler_RemoveNocIntermediateCert_BySubjectAndSKID_RevokedCertificate`
    * Remove by Subject/SKID/SerialNumber - revoked certificate:
      `TestHandler_RemoveNocIntermediateCert_BySerialNumber_RevokedCertificate`
    * Remove by Subject/SKID - revoked and active certificates:
      `TestHandler_RemoveNocIntermediateCert_BySubjectAndSKID_RevokedAndActiveCertificate`
    * Remove by Subject/SKID - another certificate with same Subject exist: ?
    * Remove by Subject/SKID - another certificate with same SKID exist: ?
    * Remove by other Vendor with the same VID: `TestHandler_RemoveNocIntermediateCert_ByNotOwnerButSameVendor`
* Negative:
    * Remove by not Vendor: `TestHandler_RemoveNocIntermediateCert_SenderNotVendor`
    * Remove not existing certificated (Subject/SKID): `TestHandler_RemoveNocIntermediateCert_CertificateDoesNotExist`
    * Remove not existing certificated (Subject/SKID + SerialNumber):
      `TestHandler_RemoveNocIntermediateCert_InvalidSerialNumber`
    * Remove NOC root certificate: `TestHandler_RemoveNocIntermediateCert_ForRoot`
    * Remove DA certificate: `TestHandler_RemoveNocIntermediateCert_ForDaCertificate`
    * Remove by other Vendor with different VID: `TestHandler_RemoveNocIntermediateCert_ByOtherVendor`
