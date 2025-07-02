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
      * [GET_ALL_PROPOSED_PAA_TO_REVOKE](#get_all_proposed_paa_to_revoke)
   * [E2E (NOC): RCAC, ICAC](#e2e_(noc):_rcac,_icac)
      * [ADD_NOC_ROOT (RCAC)](#add_noc_root_(rcac))
      * [REVOKE_NOC_ROOT (RCAC)](#revoke_noc_root_(rcac))
      * [REMOVE_NOC_ROOT (RCAC)](#remove_noc_root(rcac))
      * [ADD_NOC_ICA (ICAC)](#add_noc_ica_(icac))
      * [REVOKE_NOC_ICA (ICAC)](#revoke_noc_ica_(icac))
      * [REMOVE_NOC_ICA (ICAC)](#remove_noc_ica_(icac))
      * [GET_NOC_CERT](#get_noc_cert)
      * [GET_NOC_ROOT_BY_VID (RCACs)](#get_noc_root_by_vid_(rcacs))
      * [GET_NOC_BY_VID_AND_SKID (RCACs/ICACs)](#get_noc_by_vid_and_skid_(rcacs/icacs))
      * [GET_NOC_ICA_BY_VID (ICACs)](#get_noc_ica_by_vid_(icacs))
      * [GET_NOC_CERTS_BY_SUBJECT](#get_noc_certs_by_subject)
      * [GET_REVOKED_NOC_ROOT (RCAC)](#get_revoked_noc_root_(rcac))
      * [GET_REVOKED_NOC_ICA (ICAC)](#get_revoked_noc_ica_(icac))
      * [GET_ALL_NOC (RCACs/ICACs)](#get_all_noc_(rcacs/icacs))
      * [GET_ALL_NOC_ROOT (RCACs)](#get_all_noc_root_(rcacs))
      * [GET_ALL_NOC_ICA (ICACs)](#get_all_noc_ica_(icacs))
      * [GET_ALL_REVOKED_NOC_ROOT (RCACs)](#get_all_revoked_noc_root-(rcacs))
      * [GET_ALL_REVOKED_NOC_ICA (ICACs)](#get_all_revoked_noc_ica_(icacs))
5. [Auth](#auth)
   * [PROPOSE_ADD_ACCOUNT](#propose_add_account)
   * [APPROVE_ADD_ACCOUNT](#aprove_add_account)
   * [REJECT_ADD_ACCOUNT](#regect_add_account)
   * [PROPOSE_REVOKE_ACCOUNT](#propose_revoke_account)
   * [APPROVE_REVOKE_ACCOUNT](#approve_revoke_account)
   * [GET_ACCOUNT](#get_account)
   * [GET_PROPOSED_ACCOUNT](#get_proposed_account)
   * [GET_REJECTED_ACCOUNT](#get_rejected_account)
   * [GET_PROPOSED_ACCOUNT_TO_REVOKE](#get_proposed_account_to_revoke)
   * [GET_REVOKED_ACCOUNT](#get_revoked_account)
   * [GET_ALL_ACCOUNTS](#get_all_accounts)
   * [GET_ALL_PROPOSED_ACCOUNTS](#get_all_proposed_accounts)
   * [GET_ALL_REJECTED_ACCOUNTS](#get_all_rejected_accounts)
   * [GET_ALL_PROPOSED_ACCOUNTS_TO_REVOKE](#get_all_proposed_accounts_to_revoke)
   * [GET_ALL_REVOKED_ACCOUNTS](#get_all_revoked_accounts)
6. [Validator Node](#validator-node)
   * [ADD_VALIDATOR_NODE](#add_validator_node)
   * [DISABLE_VALIDATOR_NODE](#disable_validator_node)
   * [PROPOSE_DISABLE_VALIDATOR_NODE](#propose_disable_validator_node)
   * [APPROVE_DISABLE_VALIDATOR_NODE](#approve_disable_validator_node)
   * [REJECT_DISABLE_VALIDATOR_NODE](#reject_disable_validator_node)
   * [ENABLE_VALIDATOR_NODE](#enable_validator_node)
   * [GET_VALIDATOR](#get_validator)
   * [GET_ALL_VALIDATORS](#get_all_validators)
   * [GET_PROPOSED_DISABLE_VALIDATOR](#get_proposed_disable_validator)
   * [GET_ALL_PROPOSED_DISABLE_VALIDATORS](#get_all_proposed_disable_validators)
   * [GET_REJECTED_DISABLE_VALIDATOR](#get_rejected_disable_validator)
   * [GET_ALL_REJECTED_DISABLE_VALIDATORS](#get_all_rejected_disable_validators)
   * [GET_DISABLED_VALIDATOR](#get_disabled_validator)
   * [GET_ALL_DISABLED_VALIDATORS](#get_all_disabled_validators)
   * [GET_LAST_VALIDATOR_POWER](#get_last_validator_power)
   * [GET_ALL_LAST_VALIDATORS_POWER](#get_all_last_validators_power)
7. [Upgrade](#upgrade)
   * [PROPOSE_UPGRADE](#propose_upgrade)
   * [APPROVE_UPGRADE](#approve_upgrade)
   * [REJECT_UPGRADE](#reject_upgrade)
   * [GET_PROPOSED_UPGRADE](#get_proposed_upgrade)
   * [GET_APPROVED_UPGRADE](#get_approved_upgrade)
   * [GET_REJECTED_UPGRADE](#get_rejected_upgrade)
   * [GET_ALL_PROPOSED_UPGRADES](#get_all_proposed_upgrades)
   * [GET_ALL_APPROVED_UPGRADES](#get_all_approved_upgrades)
   * [GET_ALL_REJECTED_UPGRADES](#get_all_rejected_upgrades)
   * [GET_UPGRADE_PLAN](#get_upgrade_plan)
   * [GET_APPLIED_UPGRADE](#get_applied_upgrade)
   * [GET_MODULE_VERSIONS](#get_module_versions)

## [Vendor Info](transactions/vendor-info.md)

### [ADD_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#add_vendor_info)

#### CLI command
CLI command: `dcld tx vendorinfo add-vendor --vid=<uint16> --vendorName=<string> --companyLegalName=<string> --companyPreferredName=<string> --vendorLandingPageURL=<string> --from=<account>`

* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * access is denied to execute the command
      * multiple commands are sent with the same Vendor ID
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
         * value =< 0
         * string value format
         * length > MAX (MAX = 65535)
         * nonexistent ID
   
   * vendorName (Vendor name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative 
         * empty value
         * length > MAX
      
   * companyLegalName (Company Legal Name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative
        * empty value	
        * length > MAX

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
         * length > MAX	(MAX = 65535)

#### REST API 
POST: `/cosmos/tx/v1beta1/txs`[NewMsgCreateVendorInfo](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/proto/zigbeealliance/distributedcomplianceledger/vendorinfo/tx.proto#L18)

* REST API command send
   * Positive:
      * correct HTTP method
      * request is authorized
      * uses valid credentials/role
   * Negative:
      * incorrect request
      * multiple commands are sent with the same Vendor ID
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
         * value =< 0
         * string value format
         * length > MAX (MAX = 65535)
         * nonexistent ID
   
   * vendorName (Vendor name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative 
         * empty value	
         * length > MAX	

   * companyLegalName (Company Legal Name) - string 
      * Positive:
         * text value format	
         * MIN < length < MAX	
      * Negative
        * empty value	
        * length > MAX	

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
         * length > MAX	(MAX = 65535)

### [UPDATE_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#update_vendor_info)
#### CLI command
CLI command: `dcld tx vendorinfo update-vendor --vid=<uint16> ... --from=<account>`

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
         * value =< 0
         * string value format
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
         * length > MAX	(MAX = 65535)

#### REST API 
POST: `/cosmos/tx/v1beta1/txs`[MsgUpdateVendorInfo](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/proto/zigbeealliance/distributedcomplianceledger/vendorinfo/tx.proto#L30)

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
         * value =< 0
         * string value format
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
         * length > MAX	(MAX = 65535)

### [GET_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#get_vendor_info)
#### CLI command
CLI command: `dcld query vendorinfo vendor --vid=<uint16>`

* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
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
         * value =< 0
         * string value format
         * length > MAX (MAX = 65535)
         * nonexistent ID

#### REST API 
GET: `/dcl/vendorinfo/vendors/{vid}`

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
         * value =< 0
         * string value format
         * length > MAX (MAX = 65535)
         * nonexistent ID

### [GET_ALL_VENDOR_INFO](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/vendor-info.md#get_all_vendor_info)
#### CLI command
CLI command: `dcld query vendorinfo all-vendors`

* CLI command send
   * Positive:
      * command exists/relevant
   * Negative:
      * incorrect command syntax
      * queries are performed through a Light Client Proxy

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

* REST API command send
   * Positive:
      * correct HTTP method
      * request is authorized
      * uses valid credentials/role
   * Negative:
      * incorrect request
      * queries are performed through a Light Client Proxy
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

## [Model and Model Version]([transactions/vendor-info.md](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions.md#model-and-model-version))

### [ADD_MODEL](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/model.md#add_model)	

#### CLI command	
CLI command minimal: `dcld tx model add-model --vid=<uint16> --pid=<uint16> --deviceTypeID=<uint16> --productName=<string> --productLabel=<string or path> --partNumber=<string> --from=<account>`
CLI command full: `dcld tx model add-model --vid=<uint16> --pid=<uint16> --deviceTypeID=<uint16> --productName=<string> --productLabel=<string or path> --partNumber=<string> 
    --commissioningCustomFlow=<uint8> --commissioningCustomFlowUrl=<string> --commissioningModeInitialStepsHint=<uint32> --commissioningModeInitialStepsInstruction=<string>
    --commissioningModeSecondaryStepsHint=<uint32> --commissioningModeSecondaryStepsInstruction=<string> --userManualURL=<string> --supportURL=<string> --productURL=<string> --lsfURL=<string> --discoveryCapabilitiesBitmask=<uint16> --commissioningFallbackURL<string>
    --from=<account>`

* CLI command send	
   * Positive:
      * command exists/relevant	
   * Negative:	
      * access is denied to execute command
      * multiple commands are sent with the same unique combination of vid (vendor ID) and pid (product ID)	
      * incorrect command syntax	

* Сommand result	
  * Positive:
      * ADD_MODEL command completed successfully	**⇒** adds a new Model identified by a unique combination of vid (vendor ID) and pid (product ID)
   * Negative:	
      * ADD_MODEL command failed	**⇒** does not add a new Model identified by a unique combination of vid (vendor ID) and pid (product ID)

* Role (Who can send)
   * Positive:
      * Vendor (Vendor account associated with the given Vendor ID)
   * Negative:		
      * Trustee
      * Vendor (Vendor account is not associated with the given Vendor ID)
      * VendorAdmin 	
      * CertificationCenter 	
      * NodeAdmin 	

* Parameters:	
   
   * vid (Vendor ID) - uint16 
     * Positive:
       * unique combination	
       * value > 0	
       * integer value format
       * nonexistent ID	
     * Negative:
       * empty value	
       * value =< 0
       * string value format
       * length > MAX	(MAX = 65535)
   
   * pid (Product ID) - uint16 
     * Positive:
       * unique combination	
       * value > 0	
       * integer value format
       * nonexistent ID	
       * value falls within the specified range
     * Negative:
       * empty value
       * value =< 0
       * string value format	
       * length > MAX	(MAX = 65535)
   
   * deviceTypeID (Device Type ID) - uint16 
     * Positive:
       * value exists	
       * value >= 0	
       * integer value format
     * Negative:
       * empty value	
       * length > MAX	(MAX = 65535)
       * nonexistent ID	
   
   * productName (Product Name) - string 
     * Positive:
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * empty value	
       * length > MAX	
   
   * productLabel (Product Label) - optional(string)
     * Positive:
       * empty value	
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * length > MAX	
       * path/string format does not match	
   
   * partNumber (Part Number) - optional(string)
     * Positive:
       * empty value	
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * length > MAX	
   
   * commissioningCustomFlow (Commissioning Custom Flow) - optional(uint8)
     * Positive:
       * value exists	
       * empty value	
       * value state	
         * 1: User interaction with the device (pressing a button, for example) is required before commissioning can take place.
         * 2: The commissioner SHOULD attempt to obtain a URL which MAY be used to provide an end user with the necessary details for how to configure the product for initial commissioning 
     * Negative:
       * length > MAX	(MAX = 255)
       * nonexistent value	
   
   * commissioningCustomFlowURL (Commissioning Custom Flow URL) - optional(string)
       * commissioningCustomFlow value = '2'	
         * Positive:
           * value exists	
           * text value format	
           * MIN < length < MAX	
         * Negative:
           * length > MAX	
           * сontains spaces or line breaks	
       * commissioningCustomFlow value = '1'	
         * Positive:
           * value exists	
           * empty value	
           * text value format	
           * MIN < length < MAX	
         * Negative:
           * length > MAX	
           * сontains spaces or line breaks	
   
   * commissioningModeInitialStepsHint (Commissioning Mode Initial Steps Hint) - optional(uint32)
     * Positive:
      * value exists	
      * value >= 0	
      * integer value format
     * Negative:
      * empty value	
      * length > MAX	(MAX = 4 294 967 295)
      * value does not match Pairing Hint table	
   * commissioningModeInitialStepsInstruction (Commissioning Mode Initial Steps Instruction) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
   
   * commissioningModeSecondaryStepsHint (Commissioning Mode Secondary Steps Hint) - optional(uint32)
     * Positive:
      * value exists	
      * value >= 0	
      * integer value format
     * Negative:
      * empty value	
      * length > MAX	(MAX = 4 294 967 295)
      * inappropriate value: commissioning ModeInitialStepsInstruction text does not match selected commissioningModeInitialStepsHint value
   
   * commissioningModeSecondaryStepInstruction (Commissioning Mode Secondary Step Instruction) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * value does not match Pairing Hint table	
   
   * userManualURL (User Manual URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * User Manual URL does not match Device Type ID	
   
   * supportURL (Support URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * Support URL does not match Device Type ID	
   
   * productURL (Product URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * Product URL does not match Device Type ID	
   
   * lsfURL (Localized String File URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * Localized String File URL does not match Device Type ID	
   
   * enhancedSetupFlowOptions (Enhanced Setup Flow Options) - optional(uint16)
     * Positive:
      * value >= 0	
      * integer value format
      * empty value	
     * Negative:
      * length > MAX	(MAX = 65535)
   
   * enhancedSetupFlowTCUrl (Enhanced Setup Flow  Terms and Condition URL) - optional(string)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * empty value	
          * text value format	
          * format	
        * Negative:
          * length > MAX	
          * сontains spaces or line breaks	
          * enhancedSetupFlowTCUrl does not match Device Type ID	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCUrl field should not be present in the command	
   
   * enhancedSetupFlowTCRevision (Enhanced Setup Flow Terms and Conditions Revision) - optional(uint16)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * unique value	
          * value >= 0	
          * integer value format
          * empty value	
        * Negative:
          * length > MAX	(MAX = 65535)
          * new value < previous value	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCRevision field should not be present in the command
   
   * enhancedSetupFlowTCDigest (Enhanced Setup Flow Terms and Conditions Digest) - optional(string)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * empty value	
          * text value format	
          * MIN < length < MAX	
        * Negative:
          * length > MAX	
          * inappropriate value: digest does not match the file uploaded from the EnhancedSetupFlowTCUrl field 	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCDigest field should not be present in the command	
   
   * enhancedSetupFlowTCFileSize (Enhanced Setup Flow Terms and Conditions File Size) - optional(uint32)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * value >= 0	
          * integer value format
          * unit of measurement = bytes	
        * Negative:
          * empty value	
          * length > MAX	(MAX = 4 294 967 295)
          * enhancedSetupFlowTC file size >  EnhancedSetupFlowTCFileSize limit	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCFileSize field should not be present in the command
   
   * maintenanceUrl (Maintenance URL)	optional(string)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * empty value	
          * text value format	
          * MIN < length < MAX	
        * Negative:
          * length > MAX	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: maintenanceUrl field should not be present in the command	
   
   * schemaVersion (Schema Version) - optional(uint16)
     * Positive:
       * value = 0	
       * integer value format
       * empty value	
     * Negative:
       * length > MAX	(MAX = 65535)
   
   * discoveryCapabilitiesBitmask (Discovery Capabilities Bitmask) - optional(uint16)
     * commissioningFallbackURL field is filled	
       * Positive:
         * value = 0	
         * integer value format
         * empty value	
       * Negative:
         * length > MAX	(MAX = 65535)
     * commissioningFallbackURL field is not filled	
   
   * commissioningFallbackURL (Commissioning Fallback URL) - optional(string)
     * Positive:
       * value exists	
       * empty value	
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * length > MAX	
       * сontains spaces or line breaks	

#### REST API
REST API command:/cosmos/tx/v1beta1/txs: [MsgCreateModel](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/proto/zigbeealliance/distributedcomplianceledger/model/tx.proto#L24) 	

* REST API command send		
  * Positive:
      * correct HTTP method	
      * request is authorized	
      * uses valid credentials/role	
  * Negative:
      * incorrect request	
      * multiple commands are sent with the same unique combination of vid (vendor ID) and pid (product ID)	
      * server-side error	

* Сommand result	
  * Positive:
      * ADD_MODEL command completed successfully	**⇒** adds a new Model identified by a unique combination of vid (vendor ID) and pid (product ID)
   * Negative:	
      * ADD_MODEL command failed	**⇒** does not add a new Model identified by a unique combination of vid (vendor ID) and pid (product ID)

* Role (Who can send)
   * Positive:
      * Vendor (Vendor account associated with the given Vendor ID)
   * Negative:		
      * Trustee
      * Vendor (Vendor account is not associated with the given Vendor ID)
      * VendorAdmin 	
      * CertificationCenter 	
      * NodeAdmin 	

* Parameters:	
   
   * vid (Vendor ID) - uint16 
     * Positive:
       * unique combination	
       * value > 0	
       * integer value format
       * nonexistent ID	
     * Negative:
       * empty value	
       * length > MAX	(MAX = 65535)

   * pid (Product ID) - uint16 
     * Positive:
       * unique combination	
       * value > 0	
       * integer value format
       * nonexistent ID	
       * value falls within the specified range
     * Negative:
       * empty value	
       * length > MAX	(MAX = 65535)

   * deviceTypeID (Device Type ID) - uint16 
     * Positive:
       * value exists	
       * value >= 0	
       * integer value format
     * Negative:
       * empty value	
       * length > MAX	(MAX = 65535)
       * nonexistent ID	

   * productName (Product Name) - string 
     * Positive:
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * empty value	
       * length > MAX	
   
   * productLabel (Product Label) - optional(string)
     * Positive:
       * empty value	
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * length > MAX	
       * path/string format does not match	
   
   * partNumber (Part Number) - optional(string)
     * Positive:
       * empty value	
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * length > MAX	
   
   * commissioningCustomFlow (Commissioning Custom Flow) - optional(uint8)
     * Positive:
       * value exists	
       * empty value	
       * value state	
         * 1: User interaction with the device (pressing a button, for example) is required before commissioning can take place.
         * 2: The commissioner SHOULD attempt to obtain a URL which MAY be used to provide an end user with the necessary details for how to configure the product for initial commissioning 
     * Negative:
       * length > MAX	(MAX = 255)
       * nonexistent value	
   
   * commissioningCustomFlowURL (Commissioning Custom Flow URL) - optional(string)
       * commissioningCustomFlow value = '2'	
         * Positive:
           * value exists	
           * text value format	
           * MIN < length < MAX	
         * Negative:
           * length > MAX	
           * сontains spaces or line breaks	
       * commissioningCustomFlow value = '1'	
         * Positive:
           * value exists	
           * empty value	
           * text value format	
           * MIN < length < MAX	
         * Negative:
           * length > MAX	
           * сontains spaces or line breaks	
   
   * commissioningModeInitialStepsHint (Commissioning Mode Initial Steps Hint) - optional(uint32)
     * Positive:
      * value exists	
      * value >= 0	
      * integer value format
     * Negative:
      * empty value	
      * length > MAX	(MAX = 4 294 967 295)
      * value does not match Pairing Hint table	
   
   * commissioningModeInitialStepsInstruction (Commissioning Mode Initial Steps Instruction) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	

   * commissioningModeSecondaryStepsHint (Commissioning Mode Secondary Steps Hint) - optional(uint32)
     * Positive:
      * value exists	
      * value >= 0	
      * integer value format
     * Negative:
      * empty value	
      * length > MAX	(MAX = 4 294 967 295)
      * inappropriate value: commissioning ModeInitialStepsInstruction text does not match selected commissioningModeInitialStepsHint value
   
   * commissioningModeSecondaryStepInstruction (Commissioning Mode Secondary Step Instruction) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * value does not match Pairing Hint table	
   
   * userManualURL (User Manual URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * User Manual URL does not match Device Type ID	
   
   * supportURL (Support URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * Support URL does not match Device Type ID	

   * productURL (Product URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * Product URL does not match Device Type ID	

   * lsfURL (Localized String File URL) - optional(string)
     * Positive:
      * value exists	
      * empty value	
      * text value format	
      * MIN < length < MAX	
     * Negative:
      * length > MAX	
      * сontains spaces or line breaks	
      * Localized String File URL does not match Device Type ID	

   * enhancedSetupFlowOptions (Enhanced Setup Flow Options) - optional(uint16)
     * Positive:
      * value >= 0	
      * integer value format
      * empty value	
     * Negative:
      * length > MAX	(MAX = 65535)

   * enhancedSetupFlowTCUrl (Enhanced Setup Flow  Terms and Condition URL) - optional(string)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * empty value	
          * text value format	
          * format	
        * Negative:
          * length > MAX	
          * сontains spaces or line breaks	
          * enhancedSetupFlowTCUrl does not match Device Type ID	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set:enhancedSetupFlowTCUrl field should not be present in the command.	
   
   * enhancedSetupFlowTCRevision (Enhanced Setup Flow Terms and Conditions Revision) - optional(uint16)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * unique value	
          * value >= 0	
          * integer value format
          * empty value	
        * Negative:
          * length > MAX	(MAX = 65535)
          * new value < previous value	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCRevision field should not be present in the command.	
   
   * enhancedSetupFlowTCDigest (Enhanced Setup Flow Terms and Conditions Digest) - optional(string)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * empty value	
          * text value format	
          * MIN < length < MAX	
        * Negative:
          * length > MAX	
          * inappropriate value: digest does not match the file uploaded from the EnhancedSetupFlowTCUrl field	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCDigest field should not be present in the command
   
   * enhancedSetupFlowTCFileSize (Enhanced Setup Flow Terms and Conditions File Size) - optional(uint32)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * value >= 0	
          * integer value format
          * unit of measurement = bytes	
        * Negative:
          * empty value	
          * length > MAX	(MAX = 4 294 967 295)
          * enhancedSetupFlowTC file size >  EnhancedSetupFlowTCFileSize limit	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: enhancedSetupFlowTCFileSize field should not be present in the command

   * maintenanceUrl (Maintenance URL)	optional(string)
      * EnhancedSetupFlowOptions field has bit 0 set	
        * Positive:
          * value exists	
          * empty value	
          * text value format	
          * MIN < length < MAX	
        * Negative:
          * length > MAX	
      * EnhancedSetupFlowOptions field has bit not equal to 0 set: maintenanceUrl field should not be present in the command

   * schemaVersion (Schema Version) - optional(uint16)
     * Positive:
       * value = 0	
       * integer value format
       * empty value	
     * Negative:
       * length > MAX	(MAX = 65535)
   
   * discoveryCapabilitiesBitmask (Discovery Capabilities Bitmask) - optional(uint16)
     * commissioningFallbackURL field is filled	
       * Positive:
         * value = 0	
         * integer value format
         * empty value	
       * Negative:
         * length > MAX	(MAX = 65535)
     * commissioningFallbackURL field is not filled	
   
   * commissioningFallbackURL (Commissioning Fallback URL) - optional(string)
     * Positive:
       * value exists	
       * empty value	
       * text value format	
       * MIN < length < MAX	
     * Negative:
       * length > MAX	
       * сontains spaces or line breaks

### [EDIT_MODEL](https://github.com/zigbee-alliance/distributed-compliance-ledger/blob/master/docs/transactions/model.md#edit_model)	
#### CLI command	
CLI command send: `dcld tx model delete-model --vid=<uint16> --pid=<uint16> --from=<account>`	

* CLI command send:
  * Valid command	
    * command exists/relevant	
  * Invalid command	
    * access is denied to execute command	
    * incorrect command syntax	

* Сommand result	
  * EDIT_MODEL command completed successfully	⇒ edits an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
    * ADD_MODEL command completed successfully	
    * there is at least one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
    * combination of vid (vendor ID) and pid (product ID) valid	
    * user do not make changes to non-editable fields	
  * EDIT_MODEL command failed	⇒ does not edits an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
    * ADD_MODEL command was not executed	
    * there is not one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
    * vid (vendor ID) valid and pid (product ID) invalid	
    * vid (vendor ID) invalid and pid (product ID) valid	
    * user tries to edit non-editable fields	

* Role (Who can send)	
  * Positive:
    * Vendor (Vendor account associated with the given Vendor ID who has created the model)	
  * Negative:
    * Trustee
    * Vendor (Vendor account is not associated with the given Vendor ID who has created the model	error)
    * VendorAdmin 	
    * CertificationCenter 	
    * NodeAdmin
* Parameters:	

  * vid (Vendor ID)	uint16 
       * Positive:
  * value > 0	
  * integer value format
       * Negative:	
  * empty value
  * value =< 0
  * string value format	
  * nonexistent ID	
  * length > MAX	(MAX = 65535)
  pid (Product ID)	uint16 
       * Positive:
  value > 0	
  integer value format
  value falls within the specified range	
       * Negative:	
  empty value	
  value =< 0
  string value format	
  nonexistent ID	
  length > MAX	(MAX = 65535)
  productName (Product Name)	optional(string)
       * Positive:
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  productLabel (Product Label)	optional(string)
       * Positive:
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  path/string format does not match	
  partNumber (Part Number)	optional(string)
       * Positive:
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  nonexistent value	
  commissioningCustomFlowURL (Commissioning Custom Flow URL)	optional(string)
  commissioningCustomFlow value = '2'	
       * Positive:
  value exists	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  commissioningCustomFlow value = '1'	
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  commissioningModeInitialStepsInstruction (Commissioning Mode Initial Steps Instruction)	optional(string)
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  commissioningModeSecondaryStepInstruction (Commissioning Mode Secondary Step Instruction)	optional(string)
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  value does not match Pairing Hint table	
  userManualURL (User Manual URL)	optional(string)
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  User Manual URL does not match Device Type ID	
  supportURL (Support URL)	optional(string)
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  Support URL does not match Device Type ID	
  productURL (Product URL)	optional(string)
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  Product URL does not match Device Type ID	
  lsfURL (Localized String File URL)	optional(string)
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  Localized String File URL does not match Device Type ID	
  lsfRevision (Localized String File Revision)	optional(uint32)
       * Positive:
  value exists	
  value >= 0	
  integer value format
       * Negative:	
  empty value	
  length > MAX	(MAX = 4 294 967 295)
  nonexistent ID	
  commissioningModeInitialStepsHint (Commissioning Mode Initial Steps Hint)	optional(uint32)
       * Positive:
  value exists	
  value > 0	
  integer value format
       * Negative:	
  empty value	
  value =< 0
  string value format	
  length > MAX	MAX = (4 294 967 295)
  nonexistent ID	
  enhancedSetupFlowOptions (Enhanced Setup Flow Options)	optional(uint16)
       * Positive:
  value state	
  0	
  1	
  integer value format
  empty value	
       * Negative:	
  length > MAX	(MAX = 65535)
  enhancedSetupFlowTCUrl (Enhanced Setup Flow Terms and Condition URL)	optional(string)
  EnhancedSetupFlowOptions field has bit 0 set	
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
  enhancedSetupFlowTCUrl does not match Device Type ID	
  EnhancedSetupFlowOptions field has bit not equal to 0 set.	
  enhancedSetupFlowTCRevision (Enhanced Setup Flow Terms and Condition Revision)	optional(uint16)
  EnhancedSetupFlowOptions field has bit 0 set	
       * Positive:
  unique value	
  value >= 0	
  integer value format
  empty value	
       * Negative:	
  length > MAX	(MAX = 65535)
  new value < previous value	
  EnhancedSetupFlowOptions field has bit not equal to 0 set.	
  enhancedSetupFlowTCDigest (Enhanced Setup Flow Terms and Condition Digest)	optional(string)
  EnhancedSetupFlowOptions field has bit 0 set	
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  inappropriate value	
  EnhancedSetupFlowOptions field has bit not equal to 0 set.	
  enhancedSetupFlowTCFileSize (Enhanced Setup Flow Terms and Condition File Size)	optional(uint32)
  EnhancedSetupFlowOptions field has bit 0 set	
       * Positive:
  value exists	
  value >= 0	
  integer value format
  unit of measurement = bytes	
       * Negative:	
  empty value	
  length > MAX	(MAX = 4 294 967 295)
  enhancedSetupFlowTC file size >  EnhancedSetupFlowTCFileSize limit	
  EnhancedSetupFlowOptions field has bit not equal to 0 set.	
  maintenanceUrl (Maintenance URL)	optional(string)
  EnhancedSetupFlowOptions field has bit 0 set	
       * Positive:
  value exists	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  EnhancedSetupFlowOptions field has bit not equal to 0 set.	
  schemaVersion (Schema Version)	optional(uint16)
       * Positive:
  value exists	
  value = 0	
  integer value format
  empty value	
       * Negative:	
  length > MAX	(MAX = 65535)
  commissioningFallbackURL (Commissioning Fallback URL)	optional(string)
       * Positive:
  specific value	
  empty value	
  text value format	
  MIN < length < MAX	
       * Negative:	
  length > MAX	
  сontains spaces or line breaks	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
ADD_MODEL command was not executed	
record about a model has been deleted	
user tries to edit non-editable fields	
Сommand result	
EDIT_MODEL command completed successfully	edits an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
ADD_MODEL command completed successfully	
there is at least one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
combination of vid (vendor ID) and pid (product ID) valid	
user do not make changes to non-editable fields	
EDIT_MODEL command failed	does not edits an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
ADD_MODEL command was not executed	
there is not one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
vid (vendor ID) valid and pid (product ID) invalid	
vid (vendor ID) invalid and pid (product ID) valid	
user tries to edit non-editable fields	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor account associated with the given Vendor ID who has created the model	
Vendor account is not associated with the given Vendor ID who has created the model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent ID	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent ID	
length > MAX	(MAX = 65535)
productName (Product Name)	optional(string)
     * Positive:
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
productLabel (Product Label)	optional(string)
     * Positive:
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
path/string format does not match	
partNumber (Part Number)	optional(string)
     * Positive:
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
nonexistent value	
commissioningCustomFlowURL (Commissioning Custom Flow URL)	optional(string)
commissioningCustomFlow value = '2'	
     * Positive:
value exists	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
commissioningCustomFlow value = '1'	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
commissioningModeInitialStepsInstruction (Commissioning Mode Initial Steps Instruction)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
commissioningModeSecondaryStepInstruction (Commissioning Mode Secondary Step Instruction)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
value does not match Pairing Hint table	
userManualURL (User Manual URL)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
User Manual URL does not match Device Type ID	
supportURL (Support URL)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
Support URL does not match Device Type ID	
productURL (Product URL)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
Product URL does not match Device Type ID	
lsfURL (Localized String File URL)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
Localized String File URL does not match Device Type ID	
lsfRevision (Localized String File Revision)	optional(uint32)
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
nonexistent ID	
commissioningModeInitialStepsHint (Commissioning Mode Initial Steps Hint)	optional(uint32)
     * Positive:
value exists	
value > 0	
integer value format
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	(MAX = 4 294 967 295)
nonexistent ID	
enhancedSetupFlowOptions (Enhanced Setup Flow Options)	optional(uint16)
     * Positive:
value state	
0	
1	
integer value format
empty value	
     * Negative:	
length > MAX	(MAX = 65535)
enhancedSetupFlowTCUrl (Enhanced Setup Flow Terms and Condition URL)	optional(string)
EnhancedSetupFlowOptions field has bit 0 set	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
enhancedSetupFlowTCUrl does not match Device Type ID	
EnhancedSetupFlowOptions field has bit not equal to 0 set.	
enhancedSetupFlowTCRevision (Enhanced Setup Flow Terms and Condition Revision)	optional(uint16)
EnhancedSetupFlowOptions field has bit 0 set	
     * Positive:
unique value	
value >= 0	
integer value format
empty value	
     * Negative:	
length > MAX	(MAX = 65535)
new value < previous value	
EnhancedSetupFlowOptions field has bit not equal to 0 set.	
enhancedSetupFlowTCDigest (Enhanced Setup Flow Terms and Condition Digest)	optional(string)
EnhancedSetupFlowOptions field has bit 0 set	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
inappropriate value	
EnhancedSetupFlowOptions field has bit not equal to 0 set.	
enhancedSetupFlowTCFileSize (Enhanced Setup Flow Terms and Condition File Size)	optional(uint32)
EnhancedSetupFlowOptions field has bit 0 set	
     * Positive:
value exists	
value >= 0	
integer value format
unit of measurement = bytes	
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
enhancedSetupFlowTC file size >  EnhancedSetupFlowTCFileSize limit	
EnhancedSetupFlowOptions field has bit not equal to 0 set.	
maintenanceUrl (Maintenance URL)	optional(string)
EnhancedSetupFlowOptions field has bit 0 set	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
EnhancedSetupFlowOptions field has bit not equal to 0 set.	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:
value exists	
value = 0	
integer value format
format	
format	
format	MAX = 65535
format	optional(string)
format	
specific value	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
### DELETE_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
DELETE_MODEL command completed successfully	deletes an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
ADD_MODEL command completed successfully	
there is at least one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
combination of vid (vendor ID) and pid (product ID) valid	
the selected model has not been deleted before	
Model Versions associated with the Model is not certified	all associated Model Versions will be deleted as well
DELETE_MODEL command failed	does not deletes an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
ADD_MODEL command was not executed	
there is not one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
vid (vendor ID) valid and pid (product ID) invalid	
vid (vendor ID) invalid and pid (product ID) valid	
the selected model has been deleted before	
Model Versions associated with the Model is certified	Model can not be deleted
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor account associated with the given Vendor ID who has created the model	
Vendor account is not associated with the given Vendor ID who has created the model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent ID	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent ID	
length > MAX	(MAX = 65535)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
DELETE_MODEL command completed successfully	deletes an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
ADD_MODEL command completed successfully	
there is at least one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
combination of vid (vendor ID) and pid (product ID) valid	
the selected model has not been deleted before	
Model Versions associated with the Model is not certified	all associated Model Versions will be deleted as well
DELETE_MODEL command failed	does not deletes an existing Model identified by a unique combination of vid (vendor ID) and pid (product ID) by the vendor account
ADD_MODEL command was not executed	
there is not one Model identified by a unique combination of vid (vendor ID) and pid (product ID)	
vid (vendor ID) valid and pid (product ID) invalid	
vid (vendor ID) invalid and pid (product ID) valid	
the selected model has been deleted before	
Model Versions associated with the Model is certified	Model can not be deleted
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor account associated with the given Vendor ID who has created the model	
Vendor account is not associated with the given Vendor ID who has created the model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent ID	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent ID	
length > MAX	(MAX = 65535)
### ADD_MODEL_VERSION	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_MODEL_VERSION command completed successfully	adds a new Model Software Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion
ADD_MODEL command completed successfully	
there is at least one Model	
combination of vid (vendor ID) and pid (product ID) for Model valid	
user do not make changes to non-editable fields	
ADD_MODEL_VERSION command failed	does not adds a new Model Software Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion
ADD_MODEL command was not executed	
there is not one Model	
vid (vendor ID) valid and pid (product ID) invalid for Model	
vid (vendor ID) invalid and pid (product ID) valid for Model	
the selected model has been deleted before	
user changes to non-editable fields	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor with same Vendor ID who created the Model	
Vendor with other Vendor ID who created the Model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
softwareVersionSting (Software Version Sting)	string
     * Positive:
value exists	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
cdVersionNumber (CD Version Number)	uint16
     * Positive:
value >= 0	
integer value format
     * Negative:	
length > MAX	(MAX = 65535)
empty value	
minApplicableSoftwareVersion (Min Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value > MinApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
maxApplicableSoftwareVersion (Max Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value < maxApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
firmwareInformation (Firmware Information)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
softwareVersionValid (Software Version Valid)	optional(bool)
     * Positive:
empty value	
value state	
TRUE	
FALSE	
     * Negative:	
value is not bool	
otaURL (OTA URL)	optional(string)
OTA_checksum/OTA_checksum_type fields is set	
     * Positive:
value exists	
text value format	
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
OTA_checksum/OTA_checksum_type fields is not set	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
otaFileSize (OTA File Size)	optional(string)
     * Positive:
value exists	
empty value	
unit of measurement = bytes	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksum (OTA Checksum)	optional(string)
otaURL /OTA_checksum_type fields is set	
     * Positive:
value exists	
digest corresponds to the content of the OtaUrl attribute	
calculation method for the Digest corresponds to the algorithm from OtaChecksumType	
text value format	
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
otaURL/OTA_checksum_type fields is not set	
     * Positive:
value exists	
digest corresponds to the content of the OtaUrl attribute	
calculation method for the Digest corresponds to the algorithm from OtaChecksumType	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksumType (OTA Checksum Type)	optional(string)
otaURL /otaChecksum fields is set	
     * Positive:
value exists	
integer value format
MIN < length < MAX	
value corresponds to SHA identifier	
     * Negative:	
empty value	
length > MAX	
otaURL/otaChecksum fields is not set	
     * Positive:
value exists	
empty value	
integer value format
MIN < length < MAX	
value corresponds to SHA identifier	
     * Negative:	
length > MAX	
releaseNotesURL (Release Notes URL)	optional(string)
     * Positive:
empty value	
value exists	
URL corresponds to a specific device model	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	(MAX = 65535)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_MODEL_VERSION command completed successfully	adds a new Model Software Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion
ADD_MODEL command completed successfully	
there is at least one Model	
combination of vid (vendor ID) and pid (product ID) for Model valid	
user do not make changes to non-editable fields	
ADD_MODEL_VERSION command failed	does not adds a new Model Software Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion
ADD_MODEL command was not executed	
there is not one Model	
vid (vendor ID) valid and pid (product ID) invalid for Model	
vid (vendor ID) invalid and pid (product ID) valid for Model	
the selected model has been deleted before	
user changes to non-editable fields	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor with same Vendor ID who created the Model	
Vendor with other Vendor ID who created the Model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
softwareVersionSting (Software Version Sting)	string
     * Positive:
value exists	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
cdVersionNumber (CD Version Number)	uint16
     * Positive:
value >= 0	
integer value format
     * Negative:	
length > MAX	(MAX = 65535)
empty value	
minApplicableSoftwareVersion (Min Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value > MinApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
maxApplicableSoftwareVersion (Max Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value < maxApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
firmwareInformation (Firmware Information)	optional(string)
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
softwareVersionValid (Software Version Valid)	optional(bool)
     * Positive:
empty value	
value state	
TRUE	
FALSE	
     * Negative:	
value is not bool	
otaURL (OTA URL)	optional(string)
OTA_checksum/OTA_checksum_type fields is set	
     * Positive:
value exists	
text value format	
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
OTA_checksum/OTA_checksum_type fields is not set	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
otaFileSize (OTA File Size)	optional(string)
     * Positive:
value exists	
empty value	
unit of measurement = bytes	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksum (OTA Checksum)	optional(string)
otaURL /OTA_checksum_type fields is set	
     * Positive:
value exists	
digest corresponds to the content of the OtaUrl attribute	
calculation method for the Digest corresponds to the algorithm from OtaChecksumType	
text value format	
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
otaURL/OTA_checksum_type fields is not set	
     * Positive:
value exists	
digest corresponds to the content of the OtaUrl attribute	
calculation method for the Digest corresponds to the algorithm from OtaChecksumType	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksumType (OTA Checksum Type)	optional(string)
otaURL /otaChecksum fields is set	
     * Positive:
value exists	
integer value format
MIN < length < MAX	
value corresponds to SHA identifier	
     * Negative:	
empty value	
length > MAX	
otaURL/otaChecksum fields is not set	
     * Positive:
value exists	
empty value	
integer value format
MIN < length < MAX	
value corresponds to SHA identifier	
     * Negative:	
length > MAX	
releaseNotesURL (Release Notes URL)	optional(string)
     * Positive:
empty value	
value exists	
URL corresponds to a specific device model	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	(MAX = 65535)
### EDIT_MODEL_VERSION	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
EDIT_MODEL_VERSION command completed successfully	edits an existing Model Software Version identified by a unique combination of vid (vendor ID) pid (product ID) and softwareVersion by the vendor
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
there is at least one Model and Model Version	
combination of vid (vendor ID) and pid (product ID) for Model valid	
combination of vid (vendor ID) pid (product ID) and softwareVersion for Model Version valid	
the user did not make changes to the fields vid (vendor ID), pid (product ID) and softwareVersion	
EDIT_MODEL_VERSION command failed	does not edits an existing Model Software Version identified by a unique combination of vid (vendor ID) pid (product ID) and softwareVersion by the vendor
ADD_MODEL command was not executed	
ADD_MODEL command completed successfully, but  ADD_MODEL_VERSION command was not executed	
record about a selected Model has been deleted	
record about a selected Model Version has been deleted	
there is not one Model Version or Model	
vid (vendor ID) valid,  pid (product ID) and softwareVersion invalid	
pid (product ID) valid, vid (vendor ID) and softwareVersion invalid	
softwareVersion valid, vid (vendor ID) and pid (product ID) invalid	
user changes to non-editable fields	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor with same Vendor ID who created the Model	
Vendor with other Vendor ID who created the Model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
softwareVersionValid (Software Version Valid)	optional(bool)
     * Positive:
empty value	
value state	
TRUE	
FALSE	
     * Negative:	
value is not bool	
otaURL (OTA URL)	optional(string)
otaFileSize, otaChecksum and otaChecksumType field are already set	
     * Positive:
value exists	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
otaFileSize, otaChecksum and otaChecksumType field are not set	
maxApplicableSoftwareVersion (Max Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value < maxApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
minApplicableSoftwareVersion (Min Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value > MinApplicableSoftwareVersion value	
empty value	
length > MAX	MAX = (4 294 967 295)
otaFileSize (OTA File Size)	optional(string)
     * Positive:
value exists	
empty value	
unit of measurement = bytes	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksum (OTA Checksum)	optional(string)
     * Positive:
value exists	
digest corresponds to the content of the OtaUrl attribute	
calculation method for the Digest corresponds to the algorithm from OtaChecksumType	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksumType (OTA Checksum Type)	optional(string)
     * Positive:
value exists	
empty value	
integer value format
MIN < length < MAX	
value corresponds to SHA identifier	
     * Negative:	
length > MAX	
releaseNotesURL (Release Notes URL)	optional(string)
     * Positive:
empty value	
value exists	
URL corresponds to a specific device model	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	(MAX = 65535)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
EDIT_MODEL_VERSION command completed successfully	edits an existing Model Software Version identified by a unique combination of vid (vendor ID) pid (product ID) and softwareVersion by the vendor
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
there is at least one Model and Model Version	
combination of vid (vendor ID) and pid (product ID) for Model valid	
combination of vid (vendor ID) pid (product ID) and softwareVersion for Model Version valid	
the user did not make changes to the fields vid (vendor ID), pid (product ID) and softwareVersion	
EDIT_MODEL_VERSION command failed	does not edits an existing Model Software Version identified by a unique combination of vid (vendor ID) pid (product ID) and softwareVersion by the vendor
ADD_MODEL command was not executed	
ADD_MODEL command completed successfully, but  ADD_MODEL_VERSION command was not executed	
record about a selected Model has been deleted	
record about a selected Model Version has been deleted	
there is not one Model Version or Model	
vid (vendor ID) valid,  pid (product ID) and softwareVersion invalid	
pid (product ID) valid, vid (vendor ID) and softwareVersion invalid	
softwareVersion valid, vid (vendor ID) and pid (product ID) invalid	
user changes to non-editable fields	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor with same Vendor ID who created the Model	
Vendor with other Vendor ID who created the Model	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
softwareVersionValid (Software Version Valid)	optional(bool)
     * Positive:
empty value	
value state	
TRUE	
FALSE	
     * Negative:	
value is not bool	
otaURL (OTA URL)	optional(string)
otaFileSize, otaChecksum and otaChecksumType field are already set	
     * Positive:
value exists	
empty value	
text value format	
format	
format	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
otaFileSize, otaChecksum and otaChecksumType field are not set	
maxApplicableSoftwareVersion (Max Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value < maxApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
minApplicableSoftwareVersion (Min Applicable Software Version)	uint32
     * Positive:
value exists	
integer value format
     * Negative:	
entered value > MinApplicableSoftwareVersion value	
empty value	
length > MAX	(MAX = 4 294 967 295)
otaFileSize (OTA File Size)	optional(string)
     * Positive:
value exists	
empty value	
unit of measurement = bytes	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksum (OTA Checksum)	optional(string)
     * Positive:
value exists	
digest corresponds to the content of the OtaUrl attribute	
calculation method for the Digest corresponds to the algorithm from OtaChecksumType	
empty value	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
otaChecksumType (OTA Checksum Type)	optional(string)
     * Positive:
value exists	
empty value	
integer value format
MIN < length < MAX	
value corresponds to SHA identifier	
     * Negative:	
length > MAX	
releaseNotesURL (Release Notes URL)	optional(string)
     * Positive:
empty value	
value exists	
URL corresponds to a specific device model	
text value format	
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
incorrect URL	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	(MAX = 65535)
### DELETE_MODEL_VERSION	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
DELETE_MODEL_VERSION command completed successfully	deletes an existing Model Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion by the vendor account
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
selected Model and Model Version have not been deleted previously	
Model Version can be deleted only before it is certified	
combination of vid (vendor ID) and pid (product ID) for Model valid	
combination of vid (vendor ID) pid (product ID) and softwareVersion for Model Version valid	
DELETE_MODEL_VERSION command failed	does not deletes an existing Model Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion by the vendor account
Model Version is certified	
ADD_MODEL command was not executed	
ADD_MODEL command completed successfully, but  ADD_MODEL_VERSION command was not executed	
selected Model and Model Version have not been deleted previously	
vid (vendor ID) valid,  pid (product ID) and softwareVersion invalid	
pid (product ID) valid, vid (vendor ID) and softwareVersion invalid	
softwareVersion valid, vid (vendor ID) and pid (product ID) invalid	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor account associated with the same Vendor ID who has created the model version	
Vendor account is not associated with the same Vendor ID who has created the model version	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
DELETE_MODEL_VERSION command completed successfully	deletes an existing Model Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion by the vendor account
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
selected Model and Model Version have not been deleted previously	
Model Version can be deleted only before it is certified	
combination of vid (vendor ID) and pid (product ID) for Model valid	
combination of vid (vendor ID) pid (product ID) and softwareVersion for Model Version valid	
DELETE_MODEL_VERSION command failed	does not deletes an existing Model Version identified by a unique combination of vid (vendor ID), pid (product ID) and softwareVersion by the vendor account
Model Version is certified	
ADD_MODEL command was not executed	
ADD_MODEL command completed successfully, but  ADD_MODEL_VERSION command was not executed	
selected Model and Model Version have not been deleted previously	
vid (vendor ID) valid,  pid (product ID) and softwareVersion invalid	
pid (product ID) valid, vid (vendor ID) and softwareVersion invalid	
softwareVersion valid, vid (vendor ID) and pid (product ID) invalid	
Role (Who can send)	
Trustee	error
Vendor 	error
Vendor account associated with the same Vendor ID who has created the model version	
Vendor account is not associated with the same Vendor ID who has created the model version	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
### GET_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_MODEL command completed successfully	gets a Model Info with the given vid (vendor ID) and pid (product ID)
ADD_MODEL command completed successfully	
selected Model have not been deleted previously	
combination of vid (vendor ID) and pid (product ID) for Model valid	
GET_MODEL command failed	does not gets a Model Info with the given vid (vendor ID) and pid (product ID)
ADD_MODEL command was not executed	
record about a Model has been deleted	
vid (vendor ID) valid,  pid (product ID) invalid	
pid (product ID) valid, vid (vendor ID) invalid	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_MODEL command completed successfully	gets a Model Info with the given vid (vendor ID) and pid (product ID)
ADD_MODEL command completed successfully	
selected Model have not been deleted previously	
combination of vid (vendor ID) and pid (product ID) for Model valid	
GET_MODEL command failed	does not gets a Model Info with the given vid (vendor ID) and pid (product ID)
ADD_MODEL command was not executed	
record about a Model has been deleted	
vid (vendor ID) valid,  pid (product ID)  invalid	
pid (product ID) valid, vid (vendor ID) invalid	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
### GET_MODEL_VERSION	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_MODEL_VERSION command completed successfully	gets a Model Software Versions for the given vid, pid and softwareVersion
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
selected Model and Model Version have not been deleted previously	
combination of vid (vendor ID), pid (product ID) and softwareVersion for Model Version valid	
GET_MODEL_VERSION command failed	does not gets a Model Software Versions for the given vid, pid and softwareVersion
ADD_MODEL command was not executed	
ADD_MODEL command completed successfully, but ADD_MODEL_VERSION command was not executed	
record about a selected Model has been deleted	
record about a selected Model Version has been deleted	
vid (vendor ID) valid,  pid (product ID) and softwareVersion invalid	
pid (product ID) valid, vid (vendor ID) and softwareVersion invalid	
softwareVersion valid, vid (vendor ID) and pid (product ID) invalid	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Role (Who can send)	
Trustee	
The role corresponds to the Vendor ID	
The role is not corresponds to the Vendor ID	
Vendor 	
The role corresponds to the Vendor ID	
The role is not corresponds to the Vendor ID	
VendorAdmin 	
The role corresponds to the Vendor ID	
The role is not corresponds to the Vendor ID	
CertificationCenter 	
The role corresponds to the Vendor ID	
The role is not corresponds to the Vendor ID	
NodeAdmin 	
The role corresponds to the Vendor ID	
The role is not corresponds to the Vendor ID	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_MODEL_VERSION command completed successfully	gets a Model Software Versions for the given vid, pid and softwareVersion
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
selected Model and Model Version have not been deleted previously	
combination of vid (vendor ID), pid (product ID) and softwareVersion for Model Version valid	
GET_MODEL_VERSION command failed	does not gets a Model Software Versions for the given vid, pid and softwareVersion
ADD_MODEL command was not executed	
ADD_MODEL command completed successfully, but ADD_MODEL_VERSION command was not executed	
record about a selected Model has been deleted	
record about a selected Model Version has been deleted	
vid (vendor ID) valid,  pid (product ID) and softwareVersion invalid	
pid (product ID) valid, vid (vendor ID) and softwareVersion invalid	
softwareVersion valid, vid (vendor ID) and pid (product ID) invalid	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
pid (Product ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
softwareVersion (Software Version)	uint32
     * Positive:
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	(MAX = 4 294 967 295)
### GET_ALL_MODELS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
there is not a single model	
Сommand result	
GET_ALL_MODELS command completed successfully	gets all Model Infos for all vendors
ADD_MODEL command completed successfully	
there is at least one Model Info	
GET_ALL_MODELS command failed	does not gets all Model Infos for all vendors
ADD_MODEL command was not executed	
there is not one Model Info	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_MODELS command completed successfully	gets all Model Infos for all vendors
ADD_MODEL command completed successfully	
there is at least one Model Info	
GET_ALL_MODELS command failed	does not gets all Model Infos for all vendors
ADD_MODEL command was not executed	
there is not one Model Info	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_VENDOR_MODELS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_VENDOR_MODELS command completed successfully	gets all Model Infos by the given Vendor (vid)
ADD_MODEL command completed successfully	
there is at least one Model Info by the given Vendor (vid)	
GET_ALL_VENDOR_MODELS command failed	does not gets all Model Infos by the given Vendor (vid)
ADD_MODEL command was not executed	
there is not one Model Info by the given Vendor (vid)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	(MAX = 65535)
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_VENDOR_MODELS command completed successfully	gets all Model Infos by the given Vendor (vid)
ADD_MODEL command completed successfully	
there is at least one Model Info by the given Vendor (vid)	
GET_ALL_VENDOR_MODELS command failed	does not gets all Model Infos by the given Vendor (vid)
ADD_MODEL command was not executed	
there is not one Model Info by the given Vendor (vid)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
### GET_ALL_MODEL_VERSIONS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_MODEL_VERSIONS command completed successfully	gets all Model Software Versions for the given vid and pid combination
ADD_MODEL command completed successfully	
there is at least one Model Software Versions for the given vid and pid combination	
GET_ALL_MODEL_VERSIONS command failed	does not gets all Model Software Versions for the given vid and pid combination
ADD_MODEL command was not executed	
there is not oneModel Software Versions for the given vid and pid combination	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_MODEL_VERSIONS command completed successfully	gets all Model Software Versions for the given vid and pid combination
ADD_MODEL command completed successfully	
there is at least one Model Software Versions for the given vid and pid combination	
GET_ALL_MODEL_VERSIONS command failed	does not gets all Model Software Versions for the given vid and pid combination
ADD_MODEL command was not executed	
there is not oneModel Software Versions for the given vid and pid combination	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:
unique value	
value > 0	
integer value format
value falls within the specified range	
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
### CERTIFY_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
CERTIFY_MODEL command completed successfully	attests compliance of the Model Version to the ZB or Matter standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
corresponding Model and Model Version is present on the ledger	
command is called for compliant device for use cases where compliance is tracked on ledger	
revocation is  tracked on the ledger to remove a Model Version from the revocation list	
CERTIFY_MODEL command failed	does not attests compliance of the Model Version to the ZB or Matter standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
corresponding Model Version not present on the ledger	
corresponding Model Version is  present on the ledger, but corresponding Model not present on the ledger	
command not called for compliant device for use cases where compliance is tracked on ledger	
revocation is not tracked on the ledger to remove a Model Version from the revocation list	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
softwareVersionSting (Software Version Sting)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationDate (Certification Date)	string 
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
cDVersionNumber (CD Version Number)	optional(uint32)
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
familyId (Family ID)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
supportedClusters (Supported Clusters)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformUsed (Compliant Platform Used)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformVersion (Compliant Platform Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
OSVersion (OS Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationRoute (Certification Route)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programType (Program Type)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programTypeVersion (Program Type Version)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
transport (Transport)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
parentChild (Parent Child)	optional(string)
     * Positive:	
supported types	
parent	
child	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationIDOfSoftwareComponent (Certification ID Of Software Component)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
CERTIFY_MODEL command completed successfully	 attests compliance of the Model Version to the ZB or Matter standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
corresponding Model and Model Version is present on the ledger	
command is called for compliant device for use cases where compliance is tracked on ledger	
revocation is  tracked on the ledger to remove a Model Version from the revocation list	
CERTIFY_MODEL command failed	does not attests compliance of the Model Version to the ZB or Matter standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
corresponding Model Version not present on the ledger	
corresponding Model Version is  present on the ledger, but corresponding Model not present on the ledger	
command not called for compliant device for use cases where compliance is tracked on ledger	
revocation is not tracked on the ledger to remove a Model Version from the revocation list	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
softwareVersionSting (Software Version Sting)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationDate (Certification Date)	string 
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
cDVersionNumber (CD Version Number)	optional(uint32)
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
familyId (Family ID)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
supportedClusters (Supported Clusters)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformUsed (Compliant Platform Used)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformVersion (Compliant Platform Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
OSVersion (OS Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationRoute (Certification Route)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programType (Program Type)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programTypeVersion (Program Type Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
transport (Transport)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
parentChild (Parent Child)	optional(string)
     * Positive:	
supported types	
parent	
child	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationIDOfSoftwareComponent (Certification ID Of Software Component)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### UPDATE_COMPLIANCE_INFO	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
UPDATE_COMPLIANCE_INFO command completed successfully	updates a compliance info by VID, PID, Software Version and Certification Type
CERTIFY_MODEL command completed successfully for the selected compliance	
VID, PID, Software Version and Certification Type value are indicated correctly	
UPDATE_COMPLIANCE_INFO command failed	does not updates a compliance info by VID, PID, Software Version and Certification Type
CERTIFY_MODEL command was not executed for the selected compliance	
incorrect VID  /PID/Software Version/Certification Type	
VID, PID, Software Version values ​​are correct, Certification Type values ​​are incorrect	
VID, PID, Certification Type values ​​are correct, Software Version values ​​are incorrect	
VID, Software Version, Certification Type values ​​are correct, PID values ​​are incorrect	
Software Versio, PID, Certification Type values ​​are correct, VID values ​​are incorrect	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationDate (Certification Date)	optional(string)
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
empty value	
     * Negative:	
nonexistent value	
length > MAX	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
cDVersionNumber (CD Version Number)	optional(uint32)
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
CD version number does not match model version	
familyId (Family ID)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
supportedClusters (Supported Clusters)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformUsed (Compliant Platform Used)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformVersion (Compliant Platform Version)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
OSVersion (OS Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationRoute (Certification Route)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programType (Program Type)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programTypeVersion (Program Type Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
transport (Transport)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
parentChild (Parent Child)	optional(string)
     * Positive:	
supported types	
parent	
child	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationIDOfSoftwareComponent (Certification ID Of Software Component)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
UPDATE_COMPLIANCE_INFO command completed successfully	updates a compliance info by VID, PID, Software Version and Certification Type
CERTIFY_MODEL command completed successfully for the selected compliance	
VID, PID, Software Version and Certification Type value are indicated correctly	
UPDATE_COMPLIANCE_INFO command failed	does not updates a compliance info by VID, PID, Software Version and Certification Type
CERTIFY_MODEL command was not executed for the selected compliance	
incorrect VID  /PID/Software Version/Certification Type	
VID, PID, Software Version values ​​are correct, Certification Type values ​​are incorrect	
VID, PID, Certification Type values ​​are correct, Software Version values ​​are incorrect	
VID, Software Version, Certification Type values ​​are correct, PID values ​​are incorrect	
Software Versio, PID, Certification Type values ​​are correct, VID values ​​are incorrect	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationDate (Certification Date)	optional(string)
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
empty value	
     * Negative:	
nonexistent value	
length > MAX	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
cDVersionNumber (CD Version Number)	optional(uint32)
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
CD version number does not match model version	
familyId (Family ID)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
supportedClusters (Supported Clusters)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformUsed (Compliant Platform Used)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformVersion (Compliant Platform Version)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
OSVersion (OS Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationRoute (Certification Route)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programType (Program Type)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programTypeVersion (Program Type Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
transport (Transport)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
parentChild (Parent Child)	optional(string)
     * Positive:	
supported types	
parent	
child	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationIDOfSoftwareComponent (Certification ID Of Software Component)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### DELETE_COMPLIANCE_INFO	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
DELETE_COMPLIANCE_INFO command completed successfully	delete compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command completed successfully for the selected compliance	
there is at least one compliance of the Model Version to the ZB or Matter standard	
corresponding Compliance Info is present on the ledger	
DELETE_COMPLIANCE_INFO command failed	does not delete compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command was not executed for the selected compliance	
there is not one compliance of the Model Version to the ZB or Matter standard	
corresponding Compliance Info is not present on the ledger	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
DELETE_COMPLIANCE_INFO command completed successfully	delete compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command completed successfully for the selected compliance	
there is at least one compliance of the Model Version to the ZB or Matter standard	
corresponding Compliance Info is present on the ledger	
DELETE_COMPLIANCE_INFO command failed	does not delete compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command was not executed for the selected compliance	
there is not one compliance of the Model Version to the ZB or Matter standard	
corresponding Compliance Info is not present on the ledger	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### REVOKE_MODEL_CERTIFICATION	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REVOKE_MODEL_CERTIFICATION command completed successfully	revoke compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command completed successfully for the selected compliance	
corresponding Model and Model Version not present on the ledger	
corresponding Model and Model Version present on the ledger	
only corresponding Model present on the ledger	
only corresponding Model Version present on the ledger	
compliance result is written on the ledger	
only revocation list is stored on the ledger	
REVOKE_MODEL_CERTIFICATION command failed	does not revoke compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command was not executed for the selected compliance	
compliance result is not written on the ledger	
not only revocation list is stored on the ledger	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
softwareVersionSting (Software Version Sting)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
revocationDate (Revocation Date)	string 
     * Positive:	
format date	
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
text value format
empty value	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
Invalid command	
incorrect request	
server side error	
Сommand result	
REVOKE_MODEL_CERTIFICATION command completed successfully	revoke compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command completed successfully for the selected compliance	
corresponding Model and Model Version not present on the ledger	
corresponding Model and Model Version present on the ledger	
only corresponding Model present on the ledger	
only corresponding Model Version present on the ledger	
compliance result is written on the ledger	
only revocation list is stored on the ledger	
REVOKE_MODEL_CERTIFICATION command failed	does not revoke compliance of the Model Version to the ZB or Matter standard
CERTIFY_MODEL command was not executed for the selected compliance	
compliance result is not written on the ledger	
not only revocation list is stored on the ledger	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
softwareVersionSting (Software Version Sting)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
revocationDate (Revocation Date)	string 
     * Positive:	
format date	
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
text value format
empty value	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### PROVISION_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROVISION_MODEL command completed successfully	sets provisional state for the Model Version
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
corresponding Model and Model Version is present on the ledger	
certification record is missing from on the ledger (certified or revoked)	
PROVISION_MODEL command failed	does not sets provisional state for the Model Version
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
corresponding Model not present on the ledger	
corresponding Model is present on the ledger, but  corresponding Model Version not present on the ledger	
there is already a certification record on the ledger (certified)	
there is already a certification record on the ledger (revoked)	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
softwareVersionSting (Software Version Sting)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
provisionalDate (Provisional Date)	string 
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
cDVersionNumber (CD Version Number)	optional(uint32)
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
familyId (Family ID)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
supportedClusters (Supported Clusters)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformUsed (Compliant Platform Used)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformVersion (Compliant Platform Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
OSVersion (OS Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationRoute (Certification Route)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programType (Program Type)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programTypeVersion (Program Type Version)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
transport (Transport)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
parentChild (Parent Child)	optional(string)
     * Positive:	
supported types	
parent	
child	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationIDOfSoftwareComponent (Certification ID Of Software Component)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROVISION_MODEL command completed successfully	sets provisional state for the Model Version
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
corresponding Model and Model Version is present on the ledger	
certification record is missing from on the ledger (certified or revoked)	
PROVISION_MODEL command failed	does not sets provisional state for the Model Version
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
corresponding Model not present on the ledger	
corresponding Model is present on the ledger, but  corresponding Model Version not present on the ledger	
there is already a certification record on the ledger (certified)	
there is already a certification record on the ledger (revoked)	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
softwareVersionSting (Software Version Sting)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
provisionalDate (Provisional Date)	string 
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
reason (Reason)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
cDVersionNumber (CD Version Number)	optional(uint32)
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
familyId (Family ID)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
supportedClusters (Supported Clusters)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformUsed (Compliant Platform Used)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
compliantPlatformVersion (Compliant Platform Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
OSVersion (OS Version)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationRoute (Certification Route)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programType (Program Type)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
programTypeVersion (Program Type Version)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
transport (Transport)	optional(string)
     * Positive:	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
parentChild (Parent Child)	optional(string)
     * Positive:	
supported types	
parent	
child	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
certificationIDOfSoftwareComponent (Certification ID Of Software Component)	optional(string)
     * Positive:	
value exists	
empty value	
format	
MIN < length < MAX	
     * Negative:	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### GET_CERTIFIED_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_CERTIFIED_MODEL command completed successfully	gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is compliant to certificationType standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
compliance is tracked on the ledger	
Model Version was certified earlier	
compliance information is found on ledger and it's in certified state	
GET_CERTIFIED_MODEL command failed	does not gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is compliant to certificationType standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
a record of a Model Version is not present on the ledger	
compliance is not tracked on the ledger	
compliance  information is not found on ledger	
compliance information is found on ledger but it is not certified state	
Model Version was never certified earlier	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_CERTIFIED_MODEL command completed successfully	gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is compliant to certificationType standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
compliance is tracked on the ledger	
Model Version was certified earlier	
compliance information is found on ledger and it's in certified state	
GET_CERTIFIED_MODEL command failed	does not gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is compliant to certificationType standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
a record of a Model Version is not present on the ledger	
compliance is not tracked on the ledger	
compliance  information is not found on ledger	
compliance information is found on ledger but it is not certified state	
Model Version was never certified earlier	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
access control	
product security	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REVOKED_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REVOKED_MODEL command completed successfully	gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
only revocation is tracked on the ledger	
Model Version was certified or revoked earlier	
compliance information is found on ledger and it's in revoked state	
GET_REVOKED_MODEL command failed	does not gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
not only revocation is tracked on the ledger	
Model Version was never certified or revoked earlier	
compliance information is not found on ledger	
compliance information is found on ledger but it is not revoked state	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REVOKED_MODEL command completed successfully	gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
only revocation is tracked on the ledger	
Model Version was certified or revoked earlier	
compliance information is found on ledger and it's in revoked state	
GET_REVOKED_MODEL command failed	does not gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
not only revocation is tracked on the ledger	
Model Version was never certified or revoked earlier	
compliance information is not found on ledger	
compliance information is found on ledger but it is not revoked state	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_PROVISIONAL_MODEL	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROVISIONAL_MODEL command completed successfully	gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
Model Version was certified or revoked earlier	
compliance information is found on the ledger and it's in provisional state	
GET_PROVISIONAL_MODEL command failed	does not gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
Model Version was never certified or revoked earlier	
compliance information is not found on ledger	
compliance information is found on ledger but it is not provisional state	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROVISIONAL_MODEL command completed successfully	gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL and ADD_MODEL_VERSION command completed successfully	
a record of a Model and Model Version is present on the ledger	
Model Version was certified or revoked earlier	
compliance information is found on the ledger and it's in provisional state	
GET_PROVISIONAL_MODEL command failed	does not gets a structure containing the Model Version / Certification Type key (vid, pid, softwareVersion, certificationType) and a flag (value) indicating whether the given Model Version is revoked for certificationType standard
ADD_MODEL command was not executed	
record about a model has been removed	
ADD_MODEL command executed, but ADD_MODEL_VERSION command was not executed	
record about a model version has been removed	
Model Version was never certified or revoked earlier	
compliance information is not found on ledger	
compliance information is found on ledger but it is not provisional state	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_COMPLIANCE_INFO	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_COMPLIANCE_INFO command completed successfully	compliance information associated with the Model Version and Certification Type (identified by the vid, pid, softwareVersion and certification_type)
CERTIFY_MODEL command completed successfully for the selected compliance	
compliance information is found in store	
GET_COMPLIANCE_INFO command failed	does not gets compliance information associated with the Model Version and Certification Type (identified by the vid, pid, softwareVersion and certification_type)
CERTIFY_MODEL command was not executed for the selected compliance	
compliance information is not found in store	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value	
value =< 0
string value format	
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_COMPLIANCE_INFO command completed successfully	compliance information associated with the Model Version and Certification Type (identified by the vid, pid, softwareVersion and certification_type)
CERTIFY_MODEL command completed successfully for the selected compliance	
compliance information is found in store	
GET_COMPLIANCE_INFO command failed	does not gets compliance information associated with the Model Version and Certification Type (identified by the vid, pid, softwareVersion and certification_type)
CERTIFY_MODEL command was not executed for the selected compliance	
compliance information is not found in store	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
pid (Product ID)	uint16 
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
softwareVersion (Software Version)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
certificationType (Certification Type)	string 
     * Positive:	
existing value	
valid type	
zigbee	
matter	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_DEVICE_SOFTWARE_COMPLIANCE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_COMPLIANCE_INFO command completed successfully	gets device software compliance associated with the cDCertificateId
device software compliance is found in store	
cDCertificateId value is correct	
GET_COMPLIANCE_INFO command failed	does not gets device software compliance associated with the cDCertificateId
cDCertificateId value is incorrect	
device software compliance is not found in store	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_COMPLIANCE_INFO command completed successfully	gets device software compliance associated with the cDCertificateId
device software compliance is found in store	
cDCertificateId value is correct	
GET_COMPLIANCE_INFO command failed	does not gets device software compliance associated with the cDCertificateId
cDCertificateId value is incorrect	
device software compliance is not found in store	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
cdCertificateId (CD Certificate ID)	string 
     * Positive:	
existing value	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_CERTIFIED_MODELS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_CERTIFIED_MODELS command completed successfully	gets all compliant Model Versions for all vendors (vids)
compliance is tracked on ledger	
there is at least one compliant Model Versions for all vendors	
GET_ALL_CERTIFIED_MODELS command failed	does not gets all compliant Model Versions for all vendors (vids)
compliance is not tracked on ledger	
there is not one compliant Model Versions for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_CERTIFIED_MODELS command completed successfully	gets all compliant Model Versions for all vendors (vids)
compliance is tracked on ledger	
there is at least one compliant Model Versions for all vendors	
GET_ALL_CERTIFIED_MODELS command failed	does not gets all compliant Model Versions for all vendors (vids)
compliance is not tracked on ledger	
there is not one compliant Model Versions for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REVOKED_MODELS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REVOKED_MODELS command completed successfully	gets all revoked Model Versions for all vendors (vids)
only revocation is tracked on the ledger	
there is at least one compliant revoked Model Versions for all vendors	
GET_ALL_REVOKED_MODELS command failed	does not gets all revoked Model Versions for all vendors (vids)
not only revocation is tracked on the ledger	
there is not one compliant revoked Model Versions for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REVOKED_MODELS command completed successfully	gets all revoked Model Versions for all vendors (vids)
only revocation is tracked on the ledger	
there is at least one compliant revoked Model Versions for all vendors	
GET_ALL_REVOKED_MODELS command failed	does not gets all revoked Model Versions for all vendors (vids)
not only revocation is tracked on the ledger	
there is not one compliant revoked Model Versions for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_PROVISIONAL_MODELS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROVISIONAL_MODELS command completed successfully	gets all Model Versions in provisional state for all vendors (vids)
there is at least one Model Versions in provisional state for all vendors	
GET_ALL_PROVISIONAL_MODELS command failed	does not gets all Model Versions in provisional state for all vendors (vids)
there is at least one Model Versions in provisional state for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROVISIONAL_MODELS command completed successfully	gets all Model Versions in provisional state for all vendors (vids)
there is at least one Model Versions in provisional state for all vendors	
GET_ALL_PROVISIONAL_MODELS command failed	does not gets all Model Versions in provisional state for all vendors (vids)
there is at least one Model Versions in provisional state for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_COMPLIANCE_INFO_RECORDS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_COMPLIANCE_INFO_RECORDS command completed successfully	gets all stored compliance information records for all vendors (vids)
there is at least one stored compliance information records for all vendors	
GET_ALL_COMPLIANCE_INFO_RECORDS command failed	does not gets all stored compliance information records for all vendors (vids)
there is at least onestored compliance information records for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_COMPLIANCE_INFO_RECORDS command completed successfully	gets all stored compliance information records for all vendors (vids)
there is at least one stored compliance information records for all vendors	
GET_ALL_COMPLIANCE_INFO_RECORDS command failed	does not gets all stored compliance information records for all vendors (vids)
there is at least onestored compliance information records for all vendors	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_DEVICE_SOFTWARE_COMPLIANCES	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_DEVICE_SOFTWARE_COMPLIANCES command completed successfully	gets all stored device software compliance's
there is at least one stored device software compliance's	
GET_ALL_DEVICE_SOFTWARE_COMPLIANCES command failed	does not gets all stored device software compliance's
there is at least one stored device software compliance's	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_DEVICE_SOFTWARE_COMPLIANCES command completed successfully	gets all stored device software compliance's
there is at least one stored device software compliance's	
GET_ALL_DEVICE_SOFTWARE_COMPLIANCES command failed	does not gets all stored device software compliance's
there is at least one stored device software compliance's	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	
NodeAdmin 	error
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
All Certificates (DA, NOC)	
### GET_CERT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_CERT command completed successfully	gets a certificate by the given subject and subject key ID attributes
certificate with given subject and subject key ID attributes exists	
GET_CERT command failed	does not gets a certificate by the given subject and subject key ID attributes
certificate with given subject and subject key ID attributes not exists	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_CERT command completed successfully	gets a certificate by the given subject and subject key ID attributes
certificate with given subject and subject key ID attributes exists	
GET_CERT command failed	does not gets a certificate by the given subject and subject key ID attributes
certificate with given subject and subject key ID attributes not exists	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_CERTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_CERTS command completed successfully	gets all certificates
there is at least one certificate	
GET_ALL_CERTS command failed	does not gets all certificates
there is not a single certificate	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_CERTS command completed successfully	gets all certificates
there is at least one certificate	
GET_ALL_CERTS command failed	does not gets all certificates
there is not a single certificate	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_CERTS_BY_SUBJECT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_CERTS_BY_SUBJECT command completed successfully	gets all certificates associated with a subject
there is at least one certificate associated with a subject	
GET_ALL_CERTS_BY_SUBJECT command failed	does not gets all certificates associated with a subject
there is not one certificate associated with a subject	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_CERTS_BY_SUBJECT command completed successfully	gets all certificates associated with a subject
there is at least one certificate associated with a subject	
GET_ALL_CERTS_BY_SUBJECT command failed	does not gets all certificates associated with a subject
there is not one certificate associated with a subject	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_CERTS_BY_SKID	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_CERTS_BY_SKID command completed successfully	gets all certificates by the given subject key ID attribute
there is at least one certificate by the given subject key ID attribute	
GET_ALL_CERTS_BY_SKID command failed	does not gets all certificates by the given subject key ID attribute
there is not one certificate by the given subject key ID attribute	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
PAA	
PAI	
RCAC	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_CERTS_BY_SKID command completed successfully	gets all certificates by the given subject key ID attribute
there is at least one certificate by the given subject key ID attribute	
GET_ALL_CERTS_BY_SKID command failed	does not gets all certificates by the given subject key ID attribute
there is not one certificate by the given subject key ID attribute	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_CHILD_CERTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for child certificates	
PAI	
NOC_ICA	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_CHILD_CERTS command completed successfully	gets all child certificates for the given certificate
there is at least one child certificates for the given certificate	
GET_CHILD_CERTS command failed	does not gets all child certificates for the given certificate
there is not one child certificates for the given certificate	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for child certificates	
PAI	
NOC_ICA	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_CHILD_CERTS command completed successfully	gets all child certificates for the given certificate
there is at least one child certificates for the given certificate	
GET_CHILD_CERTS command failed	does not gets all child certificates for the given certificate
there is not one child certificates for the given certificate	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
Device Attestation Certificates (DA): PAA, PAI	
### PROPOSE_ADD_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROPOSE_ADD_PAA command completed successfully	proposes a new PAA (self-signed root certificate)
sufficient number of approvals is received	certificate added
provided certificate is root	
Issuer == Subject	
"Authority Key Identifier == Subject Key Identifier
"	
no existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exists	
the existing certificate not be NOC certificate	
"sender match to the owner of the existing certificates.
"	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
signature (self-signature) and expiration date are valid	
PROPOSE_ADD_PAA command failed	does not proposes a new PAA (self-signed root certificate)
not sufficient number of approvals is received	certificate is in Pending state
not of approvals is received	certificate not added
user tries to edit certificate	The PAA certificate is immutable
provided certificate is not root	
Issuer!= Subject, but Authority Key Identifier == Subject Key Identifier	
"Issuer == Subject, but Authority Key Identifier!= Subject Key Identifier
"	
Issuer!= Subject and Authority Key Identifier!= Subject Key Identifier	
existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
existing certificate is NOC certificate	
sender does not match to the owner of the existing certificates	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
signature (self-signature) is not valid	
signature (self-signature) is not valid and expiration date is valid	
signature (self-signature) and expiration date is not valid	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
 Who can revoked	
Trustee	
owner	if there was 1 signature for the certificate
quorum 	if there was more than 1 signature for the certificate
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
vid (Vendor ID)	uint16 
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
Vendor ID = Certificate's vid field for VID-scoped PAA	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	MAX = 65535
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROPOSE_ADD_PAA command completed successfully	proposes a new PAA (self-signed root certificate)
sufficient number of approvals is received	certificate added
provided certificate is root	
Issuer == Subject	
"Authority Key Identifier == Subject Key Identifier
"	
no existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exists	
the existing certificate not be NOC certificate	
"sender match to the owner of the existing certificates.
"	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
signature (self-signature) and expiration date are valid	
PROPOSE_ADD_PAA command failed	does not proposes a new PAA (self-signed root certificate)
not sufficient number of approvals is received	certificate is in Pending state
not of approvals is received	certificate not added
user tries to edit certificate	The PAA certificate is immutable
provided certificate is not root	
Issuer!= Subject, but Authority Key Identifier == Subject Key Identifier	
"Issuer == Subject, but Authority Key Identifier!= Subject Key Identifier
"	
Issuer!= Subject and Authority Key Identifier!= Subject Key Identifier	
existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
existing certificate is NOC certificate	
sender does not match to the owner of the existing certificates	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
signature (self-signature) is not valid	
signature (self-signature) is not valid and expiration date is valid	
signature (self-signature) and expiration date is not valid	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
 Who can revoked	
Trustee	
owner	if there was 1 signature for the certificate
quorum 	if there was more than 1 signature for the certificate
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
vid (Vendor ID)	uint16 
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
Vendor ID = Certificate's vid field for VID-scoped PAA	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	MAX = 65535
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### APPROVE_ADD_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
APPROVE_ADD_PAA command completed successfully	approves the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command completed successfully	
command used for re-voting	i.e. change vote from reject to approve
number of approvals greater than 2/3 of Trustees 	certificate active
number of approvals equal 2/3 of Trustees 	certificate active
the proposal to add a root certificate with the provided subject and subject_key_id, submitted first	
the proposed certificate hasn't been approved by the signer yet	
APPROVE_ADD_PAA command failed	does not approves the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command failed	
number of approvals is less than 2/3 of Trustees	certificate is not active
the proposal to add a root certificate with the provided subject and subject_key_id, not submitted first	
the proposed certificate has been approved by the signer	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
APPROVE_ADD_PAA command completed successfully	approves the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command completed successfully	
command used for re-voting	i.e. change vote from reject to approve
number of approvals greater than 2/3 of Trustees 	certificate active
number of approvals equal 2/3 of Trustees 	certificate active
the proposal to add a root certificate with the provided subject and subject_key_id, submitted first	
the proposed certificate hasn't been approved by the signer yet	
APPROVE_ADD_PAA command failed	does not approves the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command failed	
number of approvals is less than 2/3 of Trustees	certificate is not active
the proposal to add a root certificate with the provided subject and subject_key_id, not submitted first	
the proposed certificate has been approved by the signer	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### REJECT_ADD_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REJECT_ADD_PAA command completed successfully	rejects the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
command used for re-voting	change vote from approve to reject
remove the proposal	
proposed PAA certificate has only proposer's approval and no rejects	
number of approvals greater than 1/3 of Trustees 	certificate rejects
the proposal to add a root certificate with the provided subject and subject_key_id, submitted first	
the proposed certificate hasn't been rejected by the signer yet	
REJECT_ADD_PAA command failed	does not rejects the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
number of approvals is less than 1/3 of Trustees	certificate is not reject 
number of approvals equal 1/3 of Trustees 	certificate is not reject 
the proposal to add a root certificate with the provided subject and subject_key_id, not submitted first	
the proposed certificate has rejected by the signer	
remove the proposal	
certificate has not proposer's approval	
certificate has only proposer's approval and rejects	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
REJECT_ADD_PAA command completed successfully	rejects the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
command used for re-voting	change vote from approve to reject
remove the proposal	
proposed PAA certificate has only proposer's approval and no rejects	
number of approvals greater than 1/3 of Trustees 	certificate rejects
the proposal to add a root certificate with the provided subject and subject_key_id, submitted first	
the proposed certificate hasn't been rejected by the signer yet	
REJECT_ADD_PAA command failed	does not rejects the proposed PAA (self-signed root certificate)
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
number of approvals is less than 1/3 of Trustees	certificate is not reject 
number of approvals equal 1/3 of Trustees 	certificate is not reject 
the proposal to add a root certificate with the provided subject and subject_key_id, not submitted first	
the proposed certificate has rejected by the signer	
remove the proposal	
certificate has not proposer's approval	
certificate has only proposer's approval and rejects	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### PROPOSE_REVOKE_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROPOSE_REVOKE_PAA command completed successfully	proposes revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
revoke-child = True	all the certificates in the chain signed by the revoked certificate will be revoked as well
revoke-child = Falce	the certificates in the chain signed by the revoked certificate not be revoked
sufficient number of Trustee's approvals is received	PAA certificate is revoked
revoked certificate root	
Issuer == Subject	
Authority Key Identifier == Subject Key Identifier	
no existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
PROPOSE_REVOKE_PAA command failed	does not proposes revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
not sufficient number of Trustee's approvals is received	PAA certificate in the pending state
there are no Trustee's approvals	PAA certificate is not revoked
revoked certificate is not root	
Issuer!= Subject and Authority Key Identifier == Subject Key Identifier	
Issuer!= Subject and Authority Key Identifier!= Subject Key Identifier	
Issuer == Subject and Authority Key Identifier!= Subject Key Identifier	
existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	default value
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROPOSE_REVOKE_PAA command completed successfully	proposes revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
revoke-child = True	all the certificates in the chain signed by the revoked certificate will be revoked as well
revoke-child = Falce	the certificates in the chain signed by the revoked certificate not be revoked
sufficient number of Trustee's approvals is received	PAA certificate is revoked
revoked certificate root	
Issuer == Subject	
Authority Key Identifier == Subject Key Identifier	
no existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
PROPOSE_REVOKE_PAA command failed	does not proposes revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
not sufficient number of Trustee's approvals is received	PAA certificate in the pending state
there are no Trustee's approvals	PAA certificate is not revoked
revoked certificate is not root	
Issuer!= Subject and Authority Key Identifier == Subject Key Identifier	
Issuer!= Subject and Authority Key Identifier!= Subject Key Identifier	
Issuer == Subject and Authority Key Identifier!= Subject Key Identifier	
existing Proposed certificate with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	default value
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### APPROVE_REVOKE_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
APPROVE_REVOKE_PAA command completed successfully	approves the revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
PROPOSE_REVOKE_PAA command completed successfully	
Number of required approvals greater than 2/3 of Trustees	revocation is applied
Number of required approvals equal 2/3 of Trustees	revocation is applied
the proposal to revoke a root certificate with the provided subject and subject_key_id, submitted first	
the proposed certificate revocation hasn't been approved by the signer yet	
APPROVE_REVOKE_PAA command failed	does not approves the revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
PROPOSE_REVOKE_PAA command failed	
Number of required approvals less  than 2/3 of Trustees	revocation is not applied
the proposal to revoke a root certificate with the provided subject and subject_key_id, not submitted first	
the proposed certificate revocation has approved by the signer	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
APPROVE_REVOKE_PAA command completed successfully	approves the revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
PROPOSE_REVOKE_PAA command completed successfully	
Number of required approvals greater than 2/3 of Trustees	revocation is applied
Number of required approvals equal 2/3 of Trustees	revocation is applied
the proposal to revoke a root certificate with the provided subject and subject_key_id, submitted first	
the proposed certificate revocation hasn't been approved by the signer yet	
APPROVE_REVOKE_PAA command failed	does not approves the revocation of the given PAA (self-signed root certificate) by a Trustee
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
PROPOSE_REVOKE_PAA command failed	
Number of required approvals less  than 2/3 of Trustees	revocation is not applied
the proposal to revoke a root certificate with the provided subject and subject_key_id, not submitted first	
the proposed certificate revocation has approved by the signer	
Role	
 Who can send	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### ASSIGN_VID_TO_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ASSIGN_VID_TO_PAA command completed successfully	assigns a Vendor ID (VID) to non-VID scoped PAAs (self-signed root certificate) already present on the ledger
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
PAA Certificate with the provided subject and subject_key_id exist in the ledger	
the PAA is a VID scoped one	
the vid field equal to the VID value in the PAA's subject	
ASSIGN_VID_TO_PAA command failed	does not assigns a Vendor ID (VID) to non-VID scoped PAAs (self-signed root certificate) already present on the ledger
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
PAA Certificate with the provided subject and subject_key_id not exist in the ledger	
the PAA is a VID scoped one	
the vid field not equal to the VID value in the PAA's subject	
Role	
 Who can send	
Trustee	error
Vendor 	error
VendorAdmin 	
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = vid field in the VID-scoped PAA certificate	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	MAX = 65535
nonexistent ID	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
ASSIGN_VID_TO_PAA command completed successfully	assigns a Vendor ID (VID) to non-VID scoped PAAs (self-signed root certificate) already present on the ledger
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
PAA Certificate with the provided subject and subject_key_id exist in the ledger	
the PAA is a VID scoped one	
the vid field equal to the VID value in the PAA's subject	
ASSIGN_VID_TO_PAA command failed	does not assigns a Vendor ID (VID) to non-VID scoped PAAs (self-signed root certificate) already present on the ledger
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
PAA Certificate with the provided subject and subject_key_id not exist in the ledger	
the PAA is a VID scoped one	
the vid field not equal to the VID value in the PAA's subject	
Role	
 Who can send	
Trustee	error
Vendor 	error
VendorAdmin 	
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = vid field in the VID-scoped PAA certificate	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	MAX = 65535
nonexistent ID	
### ADD_REVOCATION_DISTRIBUTION_POINT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	publishes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
crlSignerCertificate is a PAA (root certificate)	
crlSignerCertificate is present on DCL	
crlSignerCertificate is a PAI (intermediate certificate)	
crlSignerCertificate chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is present on DCL	
crlSignerCertificate is not present on DCL	
crlSignerCertificate is a delegated by PAA	
crlSignerCertificate chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is present on DCL	
crlSignerCertificate is not present on DCL	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	does not publishes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
crlSignerCertificate is a PAA (root certificate)	
crlSignerCertificate is not present on DCL	
crlSignerCertificate is a PAI (intermediate certificate)	
crlSignerCertificate is not chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is not present on DCL	
crlSignerCertificate is a delegated by PAA	
crlSignerCertificate is not chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is not present on DCL	
Role	
 Who can send	
Trustee	error
Vendor 	
vid field in the transaction (VendorID) equal to the Vendor account's VID	
VID-scoped PAAs (Root certs) and PAIs (Intermediate certs): vid field in the CRLSignerCertificate's subject equal to the Vendor account's VID	
Non-VID scoped PAAs (Root certs): vid field associated with the corresponding PAA on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = Vendor account's VID and vid field in the VID-scoped CRLSignerCertificate	
Vendor ID value = vid associated with non-VID scoped CRLSignerCertificate on the ledger	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
pid (Product ID)	optional(uint16)
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
field is not empty if IsPAA is true	
value ≠ pid field in CRLSignerCertificate	
isPAA (Is PAA)	bool
     * Positive:	
value state	
TRUE (-1)	if the revocation information distribution point relates to a PAA
FALSE (0)	
     * Negative:	
empty value	
value is not bool	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
crlSignerCertificate (Certificate Revocation List Signer Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
crlSignerDelegator (Certificate Revocation List Signer Delegator)	optional(string)
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
certificate type	
delegated certificate by a PAI	crlSignerDelegator must contain the delegator PAI certificate which must be chained back to an approved certificate in the ledger, encoded in X.509v3 PEM format
not delegated certificate by a PAI	field can be omitted
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
dataUrl (Data Url)	string 
     * Positive:	
unique value for all pairs of VendorID and IssuerSubjectKeyID	
text value format
MIN < length < MAX	
value start with either http/https	
     * Negative:	
the format of the information does not match the format specified in the RevocationType field	
length > MAX	
empty value	
dataFileSize (Data File Size)	optional(uint64)
RevocationType ≠ 1	
     * Positive:	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	MAX = 18,446,744,073,709,551,615
RevocationType = 1	field is omitted
dataDigest (Data Digest)	optional(string)
the DataFileSize field is present	must be provided
RevocationType ≠ 1	
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
empty value	
     * Negative:	
nonexistent value	
length > MAX	
RevocationType = 1	field is omitted
the DataFileSize field is present	not must be provided
dataDigestType (Data Digest Type)	optional(uint32)
the DataDigest field is present	must be provided
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:	
value =< 0
string value format	
length > MAX	MAX = 4 294 967 295
the DataDigest field is present	not must be provided
revocationType (Revocation Type)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
supported types	1 - RFC5280 CRL
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	publishes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
crlSignerCertificate is a PAA (root certificate)	
crlSignerCertificate is present on DCL	
crlSignerCertificate is a PAI (intermediate certificate)	
crlSignerCertificate chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is present on DCL	
crlSignerCertificate is not present on DCL	
crlSignerCertificate is a delegated by PAA	
crlSignerCertificate chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is present on DCL	
crlSignerCertificate is not present on DCL	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	does not publishes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
crlSignerCertificate is a PAA (root certificate)	
crlSignerCertificate is not present on DCL	
crlSignerCertificate is a PAI (intermediate certificate)	
crlSignerCertificate is not chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is not present on DCL	
crlSignerCertificate is a delegated by PAA	
crlSignerCertificate is not chained back to a valid PAA (root certificate) present on DCL	
crlSignerCertificate is not present on DCL	
Role	
 Who can send	
Trustee	error
Vendor 	
vid field in the transaction (VendorID) equal to the Vendor account's VID	
VID-scoped PAAs (Root certs) and PAIs (Intermediate certs): vid field in the CRLSignerCertificate's subject equal to the Vendor account's VID	
Non-VID scoped PAAs (Root certs): vid field associated with the corresponding PAA on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = Vendor account's VID and vid field in the VID-scoped CRLSignerCertificate	
Vendor ID value = vid associated with non-VID scoped CRLSignerCertificate on the ledger	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
pid (Product ID)	optional(uint16)
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
value falls within the specified range	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
field is not empty if IsPAA is true	
value ≠ pid field in CRLSignerCertificate	
isPAA (Is PAA)	bool
     * Positive:	
value state	
TRUE (-1)	if the revocation information distribution point relates to a PAA
FALSE (0)	
     * Negative:	
empty value	
value is not bool	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
crlSignerCertificate (Certificate Revocation List Signer Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
crlSignerDelegator (Certificate Revocation List Signer Delegator)	optional(string)
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
certificate type	
delegated certificate by a PAI	crlSignerDelegator must contain the delegator PAI certificate which must be chained back to an approved certificate in the ledger, encoded in X.509v3 PEM format
not delegated certificate by a PAI	field can be omitted
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
dataUrl (Data Url)	string 
     * Positive:	
unique value for all pairs of VendorID and IssuerSubjectKeyID	
text value format
MIN < length < MAX	
value start with either http/https	
     * Negative:	
the format of the information does not match the format specified in the RevocationType field	
length > MAX	
empty value	
dataFileSize (Data File Size)	optional(uint64)
RevocationType ≠ 1	
     * Positive:	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	MAX = 18,446,744,073,709,551,615
RevocationType = 1	field is omitted
dataDigest (Data Digest)	optional(string)
the DataFileSize field is present	must be provided
RevocationType ≠ 1	
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
empty value	
     * Negative:	
nonexistent value	
length > MAX	
RevocationType = 1	field is omitted
the DataFileSize field is present	not must be provided
dataDigestType (Data Digest Type)	optional(uint32)
the DataDigest field is present	must be provided
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
the DataDigest field is present	not must be provided
revocationType (Revocation Type)	uint32 
     * Positive:	
value exists	
value >= 0	
integer value format
supported types	1 - RFC5280 CRL
     * Negative:	
empty value	
nonexistent value	
length > MAX	MAX = 4 294 967 295
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### UPDATE_REVOCATION_DISTRIBUTION_POINT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
UPDATE_REVOCATION_DISTRIBUTION_POINT command completed successfully	updates an existing PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
UPDATE_REVOCATION_DISTRIBUTION_POINT command failed	does not updates an existing PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	error
Vendor 	
vid field in the transaction (VendorID) equal to the Vendor account's VID	
VID-scoped PAAs (Root certs) and PAIs (Intermediate certs): vid field in the CRLSignerCertificate's subject equal to the Vendor account's VID	
Non-VID scoped PAAs (Root certs): vid field associated with the corresponding PAA on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = Vendor account's VID and vid field in the VID-scoped CRLSignerCertificate	
Vendor ID value = vid associated with non-VID scoped CRLSignerCertificate on the ledger	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
crlSignerCertificate (Certificate Revocation List Signer Certificate)	optional(string)
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
empty value	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
crlSignerDelegator (Certificate Revocation List Signer Delegator)	optional(string)
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
certificate type	
delegated certificate by a PAI	crlSignerDelegator must contain the delegator PAI certificate which must be chained back to an approved certificate in the ledger, encoded in X.509v3 PEM format
not delegated certificate by a PAI	field can be omitted
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
dataUrl (Data Url)	string 
     * Positive:	
unique value for all pairs of VendorID and IssuerSubjectKeyID	
text value format
MIN < length < MAX	
value start with either http/https	
     * Negative:	
the format of the information does not match the format specified in the RevocationType field	
length > MAX	
empty value	
dataFileSize (Data File Size)	optional(uint64)
RevocationType ≠ 1	
     * Positive:	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	MAX = 18,446,744,073,709,551,615
RevocationType = 1	field is omitted
dataDigest (Data Digest)	optional(string)
the DataFileSize field is present	must be provided
RevocationType ≠ 1	
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
empty value	
     * Negative:	
nonexistent value	
length > MAX	
RevocationType = 1	field is omitted
the DataFileSize field is present	not must be provided
dataDigestType (Data Digest Type)	optional(uint32)
the DataDigest field is present	must be provided
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
the DataDigest field is present	not must be provided
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
UPDATE_REVOCATION_DISTRIBUTION_POINT command completed successfully	updates an existing PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
UPDATE_REVOCATION_DISTRIBUTION_POINT command failed	does not updates an existing PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	error
Vendor 	
vid field in the transaction (VendorID) equal to the Vendor account's VID	
VID-scoped PAAs (Root certs) and PAIs (Intermediate certs): vid field in the CRLSignerCertificate's subject equal to the Vendor account's VID	
Non-VID scoped PAAs (Root certs): vid field associated with the corresponding PAA on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = Vendor account's VID and vid field in the VID-scoped CRLSignerCertificate	
Vendor ID value = vid associated with non-VID scoped CRLSignerCertificate on the ledger	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
crlSignerCertificate (Certificate Revocation List Signer Certificate)	optional(string)
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
empty value	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
crlSignerDelegator (Certificate Revocation List Signer Delegator)	optional(string)
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
certificate type	
delegated certificate by a PAI	crlSignerDelegator must contain the delegator PAI certificate which must be chained back to an approved certificate in the ledger, encoded in X.509v3 PEM format
not delegated certificate by a PAI	field can be omitted
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
dataUrl (Data Url)	string 
     * Positive:	
unique value for all pairs of VendorID and IssuerSubjectKeyID	
text value format
MIN < length < MAX	
value start with either http/https	
     * Negative:	
the format of the information does not match the format specified in the RevocationType field	
length > MAX	
empty value	
dataFileSize (Data File Size)	optional(uint64)
RevocationType ≠ 1	
     * Positive:	
value >= 0	
integer value format
     * Negative:	
empty value	
length > MAX	MAX = 18,446,744,073,709,551,615
RevocationType = 1	field is omitted
dataDigest (Data Digest)	optional(string)
the DataFileSize field is present	must be provided
RevocationType ≠ 1	
     * Positive:	
string matches the format	2019-10-12T07:20:50.52Z
text value format
MIN < length < MAX	
empty value	
     * Negative:	
nonexistent value	
length > MAX	
RevocationType = 1	field is omitted
the DataFileSize field is present	not must be provided
dataDigestType (Data Digest Type)	optional(uint32)
the DataDigest field is present	must be provided
     * Positive:	
value exists	
value > 0	
empty value	
format	
     * Negative:
value =< 0
string value format		
length > MAX	MAX = 4 294 967 295
the DataDigest field is present	not must be provided
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### DELETE_REVOCATION_DISTRIBUTION_POINT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
DELETE_REVOCATION_DISTRIBUTION_POINT command completed successfully	deletes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
DELETE_REVOCATION_DISTRIBUTION_POINT command failed	does not deletes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	error
Vendor 	
vid field in the transaction (VendorID) equal to the Vendor account's VID	
VID-scoped PAAs (Root certs) and PAIs (Intermediate certs): vid field in the CRLSignerCertificate's subject equal to the Vendor account's VID	
Non-VID scoped PAAs (Root certs): vid field associated with the corresponding PAA on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = Vendor account's VID and vid field in the VID-scoped CRLSignerCertificate	
Vendor ID value = vid associated with non-VID scoped CRLSignerCertificate on the ledger	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
DELETE_REVOCATION_DISTRIBUTION_POINT command completed successfully	deletes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
DELETE_REVOCATION_DISTRIBUTION_POINT command failed	does not deletes a PKI Revocation distribution endpoint (such as RFC5280 Certificate Revocation List) owned by the Vendor
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	error
Vendor 	
vid field in the transaction (VendorID) equal to the Vendor account's VID	
VID-scoped PAAs (Root certs) and PAIs (Intermediate certs): vid field in the CRLSignerCertificate's subject equal to the Vendor account's VID	
Non-VID scoped PAAs (Root certs): vid field associated with the corresponding PAA on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
Vendor ID value = Vendor account's VID and vid field in the VID-scoped CRLSignerCertificate	
Vendor ID value = vid associated with non-VID scoped CRLSignerCertificate on the ledger	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
certificate type	
delegated certificate by a PAI	must be provided using the crlSignerDelegator field
not delegated certificate by a PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
### ADD_PAI	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ADD_PAI command completed successfully	adds a PAI (intermediate certificate) signed by a chain of certificates which must be already present on the ledger
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
provided certificate not root	
Issuer != Subject	
"Authority Key Identifier != Subject Key Identifier
"	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate not be NOC certificate	
"the sender's VID match the VID of the existing certificate's owner
"	
the signature and expiration date are valid	
parent certificate already stored on the ledger and a valid chain to some root certificate can be built	
the parent root certificate is VID scoped	
the provided certificate also be VID scoped	
the vid in the subject of the root certificate equal to the vid in the subject of the provided certificate.	
the vid in the subjects of both certificates equal to the sender Vendor account's VID	
the parent root certificate is not VID scoped but has an associated VID	
the provided certificate either VID scoped or non-VID scoped	
the provided certificate is VID scoped, the vid in the subject of the certificate equal to the VID associated with the root certificate and to the sender Vendor account's VID	
multiple certificates refer to the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
ADD_PAI command failed	does not adds a PAI (intermediate certificate) signed by a chain of certificates which must be already present on the ledger
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
provided certificate is root	
Issuer == Subject	
"Authority Key Identifier == Subject Key Identifier
"	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate is NOC certificate	
"the sender's VID does not match the VID of the existing certificate's owner
"	
the signature and expiration date are not valid	
the signature is valid and expiration date are not valid	
the signature is not valid and expiration date are valid	
parent certificate not stored on the ledger	
parent certificate already stored on the ledger but a valid chain to some root certificate can not be built	
the parent root certificate is VID scoped	
the provided certificate not be VID scoped	
the vid in the subject of the root certificate not equal to the vid in the subject of the provided certificate.	
the vid in the subjects of both certificates not equal to the sender Vendor account's VID	
the parent root certificate is not VID scoped but has an associated VID	
parent root certificate is non-VID scoped and does not have an associated VID	
the provided certificate is not VID scoped	
the provided certificate is VID scoped, but the vid in the subject of the certificate not equal to the VID associated with the root certificate and to the sender Vendor account's VID	
Role	
 Who can send	
Trustee	error
Vendor 	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificate-schema-version	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_PAI command completed successfully	adds a PAI (intermediate certificate) signed by a chain of certificates which must be already present on the ledger
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
provided certificate not root	
Issuer != Subject	
"Authority Key Identifier != Subject Key Identifier
"	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate not be NOC certificate	
"the sender's VID match the VID of the existing certificate's owner
"	
the signature and expiration date are valid	
parent certificate already stored on the ledger and a valid chain to some root certificate can be built	
the parent root certificate is VID scoped	
the provided certificate also be VID scoped	
the vid in the subject of the root certificate equal to the vid in the subject of the provided certificate.	
the vid in the subjects of both certificates equal to the sender Vendor account's VID	
the parent root certificate is not VID scoped but has an associated VID	
the provided certificate either VID scoped or non-VID scoped	
the provided certificate is VID scoped, the vid in the subject of the certificate equal to the VID associated with the root certificate and to the sender Vendor account's VID	
multiple certificates refer to the same <Certificate's Subject>:<Certificate's Subject Key ID> combination	
ADD_PAI command failed	does not adds a PAI (intermediate certificate) signed by a chain of certificates which must be already present on the ledger
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
provided certificate is root	
Issuer == Subject	
"Authority Key Identifier == Subject Key Identifier
"	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate is NOC certificate	
"the sender's VID does not match the VID of the existing certificate's owner
"	
the signature and expiration date are not valid	
the signature is valid and expiration date are not valid	
the signature is not valid and expiration date are valid	
parent certificate not stored on the ledger	
parent certificate already stored on the ledger but a valid chain to some root certificate can not be built	
the parent root certificate is VID scoped	
the provided certificate not be VID scoped	
the vid in the subject of the root certificate not equal to the vid in the subject of the provided certificate.	
the vid in the subjects of both certificates not equal to the sender Vendor account's VID	
the parent root certificate is not VID scoped but has an associated VID	
parent root certificate is non-VID scoped and does not have an associated VID	
the provided certificate is not VID scoped	
the provided certificate is VID scoped, but the vid in the subject of the certificate not equal to the VID associated with the root certificate and to the sender Vendor account's VID	
Role	
 Who can send	
Trustee	error
Vendor 	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificate-schema-version	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### REVOKE_PAI	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REVOKE_PAI command completed successfully	revokes the given PAI (intermediate certificate)
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
revoke-child = True	all the certificates in the chain signed by the revoked certificate will be revoked as well
revoke-child = Falce	the certificates in the chain signed by the revoked certificate not revoked
PAI Certificate with the provided subject and subject_key_id exist in the ledger	
REVOKE_PAI command failed	does not revokes the given PAI (intermediate certificate)
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
PAI Certificate with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
sender's VID match the VID of the revoking certificate's owner	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	all the certificates in the chain signed by the revoked certificate will be revoked as well
FALSE (0)	default value
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
REVOKE_PAI command completed successfully	revokes the given PAI (intermediate certificate)
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
revoke-child = True	all the certificates in the chain signed by the revoked certificate will be revoked as well
revoke-child = Falce	the certificates in the chain signed by the revoked certificate not revoked
PAI Certificate with the provided subject and subject_key_id exist in the ledger	
REVOKE_PAI command failed	does not revokes the given PAI (intermediate certificate)
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
PAI Certificate with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
sender's VID match the VID of the revoking certificate's owner	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	all the certificates in the chain signed by the revoked certificate will be revoked as well
FALSE (0)	default value
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### REMOVE_PAI	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REMOVE_PAI command completed successfully	completely removes the given PAI (intermediate certificate) from both the approved and revoked certificates list
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
a PAI Certificate with the provided subject and subject_key_id exist in the ledger	
REMOVE_PAI command failed	does not removes the given PAI (intermediate certificate) from both the approved and revoked certificates list
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
a PAI Certificate with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
sender's VID match the VID of the removing certificate's owner	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
REMOVE_PAI command completed successfully	completely removes the given PAI (intermediate certificate) from both the approved and revoked certificates list
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
a PAI Certificate with the provided subject and subject_key_id exist in the ledger	
REMOVE_PAI command failed	does not removes the given PAI (intermediate certificate) from both the approved and revoked certificates list
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
a PAI Certificate with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
sender's VID match the VID of the removing certificate's owner	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### GET_DA_CERT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_DA_CERT command completed successfully	gets a DA certificate by the given subject and subject key ID attributes. 
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
a PAI Certificate with the provided subject and subject_key_id exist in the ledger	
GET_DA_CERT command failed	does not gets a DA certificate by the given subject and subject key ID attributes. 
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
a PAI Certificate with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_DA_CERT command completed successfully	gets a DA certificate by the given subject and subject key ID attributes. 
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_DA_CERT command failed	does not gets a DA certificate by the given subject and subject key ID attributes. 
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REVOKED_DA_CERT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REVOKED_DA_CERT command completed successfully	gets a revoked DA certificate by the given subject and subject key ID attributes
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_REVOKED_DA_CERT command failed	does not gets a revoked DA certificate by the given subject and subject key ID attributes
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REVOKED_DA_CERT command completed successfully	gets a revoked DA certificate by the given subject and subject key ID attributes
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_REVOKED_DA_CERT command failed	does not gets a revoked DA certificate by the given subject and subject key ID attributes
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_DA_CERTS_BY_SKID	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_DA_CERTS_BY_SKID command completed successfully	gets all DA certificates by the given subject key ID attribute
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_DA_CERTS_BY_SKID command failed	does not gets all DA certificates by the given subject key ID attribute
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_DA_CERTS_BY_SKID command completed successfully	gets all DA certificates by the given subject key ID attribute
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_DA_CERTS_BY_SKID command failed	does not gets all DA certificates by the given subject key ID attribute
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_DA_CERTS_BY_SUBJECT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_DA_CERTS_BY_SUBJECT command completed successfully	gets all DA certificates associated with a subject
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_DA_CERTS_BY_SUBJECT command failed	does not gets all DA certificates associated with a subject
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_DA_CERTS_BY_SUBJECT command completed successfully	gets all DA certificates associated with a subject
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_DA_CERTS_BY_SUBJECT command failed	does not gets all DA certificates associated with a subject
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_DA_CERTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_DA_CERTS command completed successfully	gets all DA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_ALL_DA_CERTS command failed	does not gets all DA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_DA_CERTS command completed successfully	gets all DA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_ALL_DA_CERTS command failed	does not gets all DA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REVOKED_DA_CERTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REVOKED_DA_CERTS command completed successfully	gets all revoked DA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_ALL_REVOKED_DA_CERTS command failed	does not gets all revoked DA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA	
PAI	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REVOKED_DA_CERTS command completed successfully	gets all revoked DA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_PAI command completed successfully	
GET_ALL_REVOKED_DA_CERTS command failed	does not gets all revoked DA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_PAI command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_PKI_REVOCATION_DISTRIBUTION_POINT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PKI_REVOCATION_DISTRIBUTION_POINT command completed successfully	gets a revocation distribution point (such as RFC5280 Certificate Revocation List) identified by (VendorID, Label, IssuerSubjectKeyID) unique combination
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
GET_PKI_REVOCATION_DISTRIBUTION_POINT command failed	does not gets a revocation distribution point (such as RFC5280 Certificate Revocation List) identified by (VendorID, Label, IssuerSubjectKeyID) unique combination
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PKI_REVOCATION_DISTRIBUTION_POINT command completed successfully	gets a revocation distribution point (such as RFC5280 Certificate Revocation List) identified by (VendorID, Label, IssuerSubjectKeyID) unique combination
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
GET_PKI_REVOCATION_DISTRIBUTION_POINT command failed	does not gets a revocation distribution point (such as RFC5280 Certificate Revocation List) identified by (VendorID, Label, IssuerSubjectKeyID) unique combination
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
value exists	
value > 0	
integer value format
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
nonexistent ID	
label (Label)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
### GET_PKI_REVOCATION_DISTRIBUTION_POINTS_BY_SUBJECT_KEY_ID	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PKI_REVOCATION_DISTRIBUTION_POINTS_BY_SUBJECT_KEY_ID command completed successfully	gets a list of revocation distribution point (such as RFC5280 Certificate Revocation List) identified by IssuerSubjectKeyID
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
GET_PKI_REVOCATION_DISTRIBUTION_POINTS_BY_SUBJECT_KEY_ID command failed	does not gets a a list of revocation distribution point (such as RFC5280 Certificate Revocation List) identified by IssuerSubjectKeyID
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PKI_REVOCATION_DISTRIBUTION_POINTS_BY_SUBJECT_KEY_ID command completed successfully	gets a list of revocation distribution point (such as RFC5280 Certificate Revocation List) identified by IssuerSubjectKeyID
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
GET_PKI_REVOCATION_DISTRIBUTION_POINTS_BY_SUBJECT_KEY_ID command failed	does not gets a a list of revocation distribution point (such as RFC5280 Certificate Revocation List) identified by IssuerSubjectKeyID
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
issuerSubjectKeyID (Issuer Subject Key ID)	string 
     * Positive:	
unique value for PAA/PAI	
text value format
MIN < length < MAX	
value consist of even number of uppercase hexadecimal characters ([0-9A-F])	for example, 5A880E6C3653D07FB08971A3F473790930E62BDB
     * Negative:	
contains whitespace	
contains non-hexadecimal characters	
length > MAX	
empty value	
### GET_ALL_PKI_REVOCATION_DISTRIBUTION_POINT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PKI_REVOCATION_DISTRIBUTION_POINT command completed successfully	gets a list of all revocation distribution points (such as RFC5280 Certificate Revocation List)
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
GET_ALL_PKI_REVOCATION_DISTRIBUTION_POINT command failed	does not gets a list of all revocation distribution points (such as RFC5280 Certificate Revocation List)
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PKI_REVOCATION_DISTRIBUTION_POINT command completed successfully	gets a list of all revocation distribution points (such as RFC5280 Certificate Revocation List)
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
ADD_REVOCATION_DISTRIBUTION_POINT command completed successfully	
GET_ALL_PKI_REVOCATION_DISTRIBUTION_POINT command failed	does not gets a list of all revocation distribution points (such as RFC5280 Certificate Revocation List)
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
ADD_REVOCATION_DISTRIBUTION_POINT command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_PROPOSED_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of certificates	
PAA	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROPOSED_PAA command completed successfully	gets a proposed but not approved PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command completed successfully	
GET_PROPOSED_PAA command failed	does not gets a proposed but not approved PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command failed	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
PAA	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROPOSED_PAA command completed successfully	gets a proposed but not approved PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command completed successfully	
GET_PROPOSED_PAA command failed	does not gets a proposed but not approved PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command failed	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REJECTED_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of certificates	
PAA	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REJECTED_PAA command completed successfully	gets a rejected PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command completed successfully, but PAA certificate rejected	
there is at least one rejected PAA certificate	
GET_REJECTED_PAA command failed	does not gets a rejected PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command failed	
there are not one rejected PAA certificates	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
PAA	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REJECTED_PAA command completed successfully	gets a rejected PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command completed successfully, but PAA certificate rejected	
there is at least one rejected PAA certificate	
GET_REJECTED_PAA command failed	does not gets a rejected PAA certificate with the given subject and subject key ID attributes
PROPOSE_ADD_PAA command failed	
there are not one rejected PAA certificates	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_PROPOSED_PAA_TO_REVOKE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROPOSED_PAA_TO_REVOKE command completed successfully	gets a proposed but not approved PAA certificate to be revoked
PROPOSE_ADD_PAA command completed successfully, but PAA certificate not approved	
there is at least one not approved  PAA certificate	
GET_PROPOSED_PAA_TO_REVOKE command failed	does not gets a proposed but not approved PAA certificate to be revoked
PROPOSE_ADD_PAA command failed	
there are not one not approved PAA certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROPOSED_PAA_TO_REVOKE command completed successfully	gets a proposed but not approved PAA certificate to be revoked
PROPOSE_ADD_PAA command completed successfully, but PAA certificate not approved	
there is at least one not approved  PAA certificate	
GET_PROPOSED_PAA_TO_REVOKE command failed	does not gets a proposed but not approved PAA certificate to be revoked
PROPOSE_ADD_PAA command failed	
there are not one not approved PAA certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### GET_ALL_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PAA command completed successfully	gets all approved PAA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
there is at least one approved  PAA certificate	
GET_ALL_PAA command failed	does not gets all approved PAA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
there are not one approved PAA certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PAA command completed successfully	gets all approved PAA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
there is at least one approved  PAA certificate	
GET_ALL_PAA command failed	does not gets all approved PAA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
there are not one approved PAA certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REVOKED_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REVOKED_PAA command completed successfully	gets all revoked PAA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
PROPOSE_REVOKE_PAA command completed successfully	
APPROVE_REVOKE_PAA command completed successfully	
there is at least one revoked PAA certificates	
GET_ALL_REVOKED_PAA command failed	does not gets all revoked PAA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
PROPOSE_REVOKE_PAA command failed	
APPROVE_REVOKE_PAA command failed	
there are not one revoked PAA certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REVOKED_PAA command completed successfully	gets all revoked PAA certificates
PROPOSE_ADD_PAA command completed successfully	
APPROVE_ADD_PAA command completed successfully	
PROPOSE_REVOKE_PAA command completed successfully	
APPROVE_REVOKE_PAA command completed successfully	
there is at least one revoked PAA certificates	
GET_ALL_REVOKED_PAA command failed	does not gets all revoked PAA certificates
PROPOSE_ADD_PAA command failed	
APPROVE_ADD_PAA command failed	
PROPOSE_REVOKE_PAA command failed	
APPROVE_REVOKE_PAA command failed	
there are not one revoked PAA certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_PROPOSED_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROPOSED_PAA command completed successfully	gets all proposed but not approved root certificates
PROPOSE_ADD_PAA command completed successfully, but not approved root certificates	
there is at least one proposed but not approved root certificates	
GET_ALL_PROPOSED_PAA command failed	does not gets all proposed but not approved root certificates
PROPOSE_ADD_PAA command failed	
there are not one proposed but not approved root certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROPOSED_PAA command completed successfully	gets all proposed but not approved root certificates
PROPOSE_ADD_PAA command completed successfully, but not approved root certificates	
there is at least one proposed but not approved root certificates	
GET_ALL_PROPOSED_PAA command failed	does not gets all proposed but not approved root certificates
PROPOSE_ADD_PAA command failed	
there are not one proposed but not approved root certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REJECTED_PAA	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REJECTED_PAA command completed successfully	gets all rejected root certificates
PROPOSE_ADD_PAA command completed successfully, but root certificates rejected 	
there is at least one rejected root certificates	
GET_ALL_REJECTED_PAA command failed	does not gets all rejected root certificates
PROPOSE_ADD_PAA command failed	
there are not one rejected root certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REJECTED_PAA command completed successfully	gets all rejected root certificates
PROPOSE_ADD_PAA command completed successfully, but root certificates rejected 	
there is at least one rejected root certificates	
GET_ALL_REJECTED_PAA command failed	does not gets all rejected root certificates
PROPOSE_ADD_PAA command failed	
there are not one rejected root certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_PROPOSED_PAA_TO_REVOKE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
PAA 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROPOSED_PAA_TO_REVOKE command completed successfully	gets all proposed but not approved root certificates to be revoked
PROPOSE_ADD_PAA command completed successfully, but root certificates not approved 	
there is at least one proposed but not approved root certificates	
GET_ALL_PROPOSED_PAA_TO_REVOKE command failed	does not gets all proposed but not approved root certificates to be revoked
PROPOSE_ADD_PAA command failed	
there are not one proposed but not approved root certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
PAA 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROPOSED_PAA_TO_REVOKE command completed successfully	gets all proposed but not approved root certificates to be revoked
PROPOSE_ADD_PAA command completed successfully, but root certificates not approved 	
there is at least one proposed but not approved root certificates	
GET_ALL_PROPOSED_PAA_TO_REVOKE command failed	does not gets all proposed but not approved root certificates to be revoked
PROPOSE_ADD_PAA command failed	
there are not one proposed but not approved root certificates	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
E2E (NOC): RCAC, ICAC	
### ADD_NOC_ROOT (RCAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
RCAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ADD_NOC_ROOT (RCAC) command completed successfully	adds a NOC root certificate (RCAC) owned by the Vendor
the provided certificate be a root certificate (RCAC)	
Issuer == Subject	
"Authority Key Identifier == Subject Key Identifier
"	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate NOC root certificate (RCAC)	
"the sender's VID match the vid field of the existing certificates
"	
the signature (self-signature) and expiration date must be valid	
ADD_NOC_ROOT (RCAC) command failed	does not adds a NOC root certificate (RCAC) owned by the Vendor
the provided certificate not a root certificate (RCAC)	
Issuer!= Subject and Authority Key Identifier == Subject Key Identifier	
"Issuer!= Subject  and Authority Key Identifier != Subject Key Identifier
"	
"Issuer == Subject  and Authority Key Identifier == Subject Key Identifier
"	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate is not NOC root certificate (RCAC)	
"the sender's VID is not match the vid field of the existing certificates
"	
the signature (self-signature) and expiration date not be valid	
the signature (self-signature) is valid and expiration date not be valid	
the signature (self-signature) not be valid and expiration date valid	
Role	
 Who can send	
Trustee	error
Vendor 	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
RCAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_NOC_ROOT (RCAC) command completed successfully	adds a NOC root certificate (RCAC) owned by the Vendor
the provided certificate be a root certificate (RCAC)	
Issuer == Subject	
"Authority Key Identifier == Subject Key Identifier
"	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate NOC root certificate (RCAC)	
"the sender's VID match the vid field of the existing certificates
"	
the signature (self-signature) and expiration date must be valid	
ADD_NOC_ROOT (RCAC) command failed	does not adds a NOC root certificate (RCAC) owned by the Vendor
the provided certificate not a root certificate (RCAC)	
Issuer!= Subject and Authority Key Identifier == Subject Key Identifier	
"Issuer!= Subject  and Authority Key Identifier != Subject Key Identifier
"	
"Issuer == Subject  and Authority Key Identifier == Subject Key Identifier
"	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate is not NOC root certificate (RCAC)	
"the sender's VID is not match the vid field of the existing certificates
"	
the signature (self-signature) and expiration date not be valid	
the signature (self-signature) is valid and expiration date not be valid	
the signature (self-signature) not be valid and expiration date valid	
Role	
 Who can send	
Trustee	error
Vendor 	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
schemaVersion (Schema Version)	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### REVOKE_NOC_ROOT (RCAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
RCAC 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REVOKE_NOC_ROOT (RCAC) command completed successfully	revokes a NOC root certificate (RCAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id exist in the ledger	
REVOKE_NOC_ROOT (RCAC) command failed	does not revokes a NOC root certificate (RCAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command failed	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id is not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC root certificate (RCAC) on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	then all certificates in the chain signed by the revoked certificate (intermediate, leaf) are revoked as well
FALSE (0)	only the current root cert is revoked (default value)
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
RCAC 	
Invalid command	
incorrect request	
server side error	
Сommand result	
REVOKE_NOC_ROOT (RCAC) command completed successfully	revokes a NOC root certificate (RCAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id exist in the ledger	
REVOKE_NOC_ROOT (RCAC) command failed	does not revokes a NOC root certificate (RCAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command failed	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id is not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC root certificate (RCAC) on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	then all certificates in the chain signed by the revoked certificate (intermediate, leaf) are revoked as well
FALSE (0)	only the current root cert is revoked (default value)
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### REMOVE_NOC_ROOT (RCAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
RCAC 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REMOVE_NOC_ROOT (RCAC) command completed successfully	completely removes the given NOC root certificate (RCAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id exist in the ledger	
REMOVE_NOC_ROOT (RCAC) command failed	does not completely removes the given NOC root certificate (RCAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command failed	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC certificate on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
RCAC 	
Invalid command	
incorrect request	
server side error	
Сommand result	
REMOVE_NOC_ROOT (RCAC) command completed successfully	completely removes the given NOC root certificate (RCAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id exist in the ledger	
REMOVE_NOC_ROOT (RCAC) command failed	does not completely removes the given NOC root certificate (RCAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command failed	
a NOC Root Certificate (RCAC) with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC certificate on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### ADD_NOC_ICA (ICAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ADD_NOC_ICA (ICAC) command completed successfully	adds a NOC ICA certificate (ICAC) owned by the Vendor signed by a chain of certificates which must be already present on the ledger
ADD_NOC_ROOT (RCAC) command completed successfully	
the certificate chain is already present in the ledger	
"the provided certificate a non-root certificate
"	
Issuer != Subject	
Authority Key Identifier != Subject Key Identifier	
the root certificate e a NOC certificate and added by the same vendor	
isNoc field of the root certificate set to true	
VID of root certificate == VID of account	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate NOC non-root certificate	
the sender's VID match the vid field of the existing certificates	
the signature and expiration date valid	
ADD_NOC_ICA (ICAC) command failed	does not adds a NOC ICA certificate (ICAC) owned by the Vendor signed by a chain of certificates which must be already present on the ledger
ADD_NOC_ROOT (RCAC) command failed	
the certificate chain is not present in the ledger	
"the provided certificate a root certificate
"	
Issuer != Subject and Authority Key Identifier == Subject Key Identifier	
Issuer == Subject and Authority Key Identifier != Subject Key Identifier	
Issuer == Subject and Authority Key Identifier == Subject Key Identifier	
the root certificate is not NOC certificate and added by the same vendor	
isNoc field of the root certificate is not set to true	
VID of root certificate != VID of account	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate NOC root certificate	
the sender's VID does not match the vid field of the existing certificates	
the signature and expiration date invalid	
the signature invalid and expiration date valid	
the signature valid and expiration date invalid	
Role	
 Who can send	
Trustee	error
Vendor 	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificate-schema-version	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_NOC_ICA (ICAC) command completed successfully	adds a NOC ICA certificate (ICAC) owned by the Vendor signed by a chain of certificates which must be already present on the ledger
ADD_NOC_ROOT (RCAC) command completed successfully	
the certificate chain is already present in the ledger	
"the provided certificate a non-root certificate
"	
Issuer != Subject	
Authority Key Identifier != Subject Key Identifier	
the root certificate e a NOC certificate and added by the same vendor	
isNoc field of the root certificate set to true	
VID of root certificate == VID of account	
no existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate NOC non-root certificate	
the sender's VID match the vid field of the existing certificates	
the signature and expiration date valid	
ADD_NOC_ICA (ICAC) command failed	does not adds a NOC ICA certificate (ICAC) owned by the Vendor signed by a chain of certificates which must be already present on the ledger
ADD_NOC_ROOT (RCAC) command failed	
the certificate chain is not present in the ledger	
"the provided certificate a root certificate
"	
Issuer != Subject and Authority Key Identifier == Subject Key Identifier	
Issuer == Subject and Authority Key Identifier != Subject Key Identifier	
Issuer == Subject and Authority Key Identifier == Subject Key Identifier	
the root certificate is not NOC certificate and added by the same vendor	
isNoc field of the root certificate is not set to true	
VID of root certificate != VID of account	
existing certificate with the same <Certificate's Issuer>:<Certificate's Serial Number> combination	
certificates with the same <Certificate's Subject>:<Certificate's Subject Key ID> combination already exist	
the existing certificate NOC root certificate	
the sender's VID does not match the vid field of the existing certificates	
the signature and expiration date invalid	
the signature invalid and expiration date valid	
the signature valid and expiration date invalid	
Role	
 Who can send	
Trustee	error
Vendor 	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
cert (Certificate)	string 
     * Positive:	
value exists	
contain a PEM string	
contain path to a file containing the data	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
certificate-schema-version	optional(uint16)
     * Positive:	
value = 0	
integer value format
empty value	
     * Negative:	
length > MAX	MAX = 65535
### REVOKE_NOC_ICA (ICAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REVOKE_NOC_ICA (ICAC) command completed successfully	revokes a NOC ICA certificate (ICAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC Certificate with the provided subject and subject_key_id exist in the ledger	
REVOKE_NOC_ICA (ICAC) command failed	does not revokes a NOC ICA certificate (ICAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command failed	
a NOC Certificate with the provided subject and subject_key_id is not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC certificate on the ledger must be equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	all certificates in the chain signed by the revoked certificate (leaf) are revoked as well
FALSE (0)	only the current cert is revoked (default value)
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
REVOKE_NOC_ICA (ICAC) command completed successfully	revokes a NOC ICA certificate (ICAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC Certificate with the provided subject and subject_key_id exist in the ledger	
REVOKE_NOC_ICA (ICAC) command failed	does not revokes a NOC ICA certificate (ICAC) owned by the Vendor
ADD_NOC_ROOT (RCAC) command failed	
a NOC Certificate with the provided subject and subject_key_id is not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC certificate on the ledger must be equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
revoke-child (Revoke Child)	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	all certificates in the chain signed by the revoked certificate (leaf) are revoked as well
FALSE (0)	only the current cert is revoked (default value)
     * Negative:	
value is not bool	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	MAX=4096 characters
time (Proposal Time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### REMOVE_NOC_ICA (ICAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for  the following certificates	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REMOVE_NOC_ICA (ICAC) command completed successfully	completely removes the given NOC ICA (ICAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC ICA Certificate (ICAC) with the provided subject and subject_key_id exist in the ledger	
REMOVE_NOC_ICA (ICAC) command failed	does not removes the given NOC ICA (ICAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command failed	
a NOC ICA Certificate (ICAC) with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC certificate on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for  the following certificates	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
REMOVE_NOC_ICA (ICAC) command completed successfully	completely removes the given NOC ICA (ICAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command completed successfully	
a NOC ICA Certificate (ICAC) with the provided subject and subject_key_id exist in the ledger	
REMOVE_NOC_ICA (ICAC) command failed	does not removes the given NOC ICA (ICAC) owned by the Vendor from the ledger
ADD_NOC_ROOT (RCAC) command failed	
a NOC ICA Certificate (ICAC) with the provided subject and subject_key_id not exist in the ledger	
Role	
 Who can send	
Trustee	error
Vendor 	
Vid field associated with the corresponding NOC certificate on the ledger equal to the Vendor account's VID	
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
serial-number (Serial Number)	optional(string)
     * Positive:	
empty value	
transaction will revoke all certificates that match the given subject and subject_key_id combination	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### GET_NOC_CERT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of Noc certificates	
NOC_ROOT	
NOC_ICA	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_NOC_CERT command completed successfully	gets a NOC certificate by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_CERT command failed	does not gets a NOC certificate by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of Noc certificates	
NOC_ROOT	
NOC_ICA	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_NOC_CERT command completed successfully	gets a NOC certificate by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_CERT command failed	does not gets a NOC certificate by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_NOC_ROOT_BY_VID (RCACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of Noc certificates	
RCACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_NOC_ROOT_BY_VID (RCACs) command completed successfully	retrieve NOC root certificates (RCACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_ROOT_BY_VID (RCACs) command failed	does not retrieve NOC root certificates (RCACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of Noc certificates	
RCACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_NOC_ROOT_BY_VID (RCACs) command completed successfully	retrieve NOC root certificates (RCACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_ROOT_BY_VID (RCACs) command failed	does not retrieve NOC root certificates (RCACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
### GET_NOC_BY_VID_AND_SKID (RCACs/ICACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of Noc certificates	
RCACs	
ICACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_NOC_BY_VID_AND_SKID (RCACs/ICACs) command completed successfully	retrieve NOC (Root/ICA) certificates (RCACs/ICACs) associated with a specific VID and subject key ID
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_BY_VID_AND_SKID (RCACs/ICACs) command failed	does not retrieve NOC (Root/ICA) certificates (RCACs/ICACs) associated with a specific VID and subject key ID
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of Noc certificates	
RCACs	
ICACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_NOC_BY_VID_AND_SKID (RCACs/ICACs) command completed successfully	retrieve NOC (Root/ICA) certificates (RCACs/ICACs) associated with a specific VID and subject key ID
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_BY_VID_AND_SKID (RCACs/ICACs) command failed	does not retrieve NOC (Root/ICA) certificates (RCACs/ICACs) associated with a specific VID and subject key ID
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_NOC_ICA_BY_VID (ICACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for all types of Noc certificates	
ICACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_NOC_ICA_BY_VID (ICACs) command completed successfully	retrieve NOC ICA certificates (ICACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_ICA_BY_VID (ICACs) command failed	does not retrieve NOC ICA certificates (ICACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of Noc certificates	
ICACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_NOC_ICA_BY_VID (ICACs) command completed successfully	retrieve NOC ICA certificates (ICACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_ICA_BY_VID (ICACs) command failed	does not retrieve NOC ICA certificates (ICACs) associated with a specific VID
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
vid (Vendor ID)	uint16
     * Positive:	
unique value	
value > 0	
integer value format
     * Negative:	
empty value
value =< 0
string value format		
nonexistent value	
length > MAX	MAX = 65535
### GET_NOC_CERTS_BY_SUBJECT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for both types of certificates	
NOC_ROOT	
NOC_ICA	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_NOC_CERTS_BY_SUBJECT command completed successfully	gets all NOC certificates associated with a subject
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_CERTS_BY_SUBJECT command failed	does not gets all NOC certificates associated with a subject
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for both types of certificates	
NOC_ROOT	
NOC_ICA	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_NOC_CERTS_BY_SUBJECT command completed successfully	gets all NOC certificates associated with a subject
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_NOC_CERTS_BY_SUBJECT command failed	does not gets all NOC certificates associated with a subject
ADD_NOC_ROOT (RCAC) command failed	
Role	
 Who can send	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REVOKED_NOC_ROOT (RCAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
RCAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REVOKED_NOC_ROOT (RCAC) command completed successfully	gets a revoked NOC root certificate (RCAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_REVOKED_NOC_ROOT (RCAC) command failed	does not gets a revoked NOC root certificate (RCAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command failed	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
RCAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REVOKED_NOC_ROOT (RCAC) command completed successfully	gets a revoked NOC root certificate (RCAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_REVOKED_NOC_ROOT (RCAC) command failed	does not gets a revoked NOC root certificate (RCAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command failed	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REVOKED_NOC_ICA (ICAC)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
ICAC	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REVOKED_NOC_ICA (ICAC) command completed successfully	gets a revoked NOC ica certificate (ICAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_REVOKED_NOC_ICA (ICAC) command failed	does not a revoked NOC ica certificate (ICAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command failed	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for all types of certificates	
ICAC	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REVOKED_NOC_ICA (ICAC) command completed successfully	gets a revoked NOC ica certificate (ICAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command completed successfully	
GET_REVOKED_NOC_ICA (ICAC) command failed	does not a revoked NOC ica certificate (ICAC) by the given subject and subject key ID attributes
ADD_NOC_ROOT (RCAC) command failed	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
subject (Subject)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
subject_key_id (Subject Key ID)	string 
     * Positive:	
string matches the format	for example: 5A:88:0E:6C:36:53:D0:7F:B0:89:71:A3:F4:73:79:09:30:E6:2B:DB
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_NOC (RCACs/ICACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
RCACs 	
ICACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_NOC (RCACs/ICACs) command completed successfully	retrieve a list of all of NOC certificates (RCACs of ICACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one NOC certificates (RCACs of ICACs)	
GET_ALL_NOC (RCACs/ICACs) command failed	does not retrieve a list of all of NOC certificates (RCACs of ICACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one NOC certificates (RCACs of ICACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for following certificates	
RCACs 	
ICACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_NOC (RCACs/ICACs) command completed successfully	retrieve a list of all of NOC certificates (RCACs of ICACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one NOC certificates (RCACs of ICACs)	
GET_ALL_NOC (RCACs/ICACs) command failed	does not retrieve a list of all of NOC certificates (RCACs of ICACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one NOC certificates (RCACs of ICACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_NOC_ROOT (RCACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
RCACs 	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_NOC_ROOT (RCACs) command completed successfully	retrieve a list of all of NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one NOC root certificates (RCACs)	
GET_ALL_NOC_ROOT (RCACs) command failed	does not retrieve a list of all of NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one NOC root certificates (RCACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for following certificates	
RCACs 	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_NOC_ROOT (RCACs) command completed successfully	retrieve a list of all of NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one NOC root certificates (RCACs)	
GET_ALL_NOC_ROOT (RCACs) command failed	does not retrieve a list of all of NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one NOC root certificates (RCACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_NOC_ICA (ICACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
ICACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_NOC_ICA (ICACs) command completed successfully	retrieve a list of all of NOC ICA certificates (ICACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one NOC ICA certificates (ICACs)	
GET_ALL_NOC_ICA (ICACs) command failed	does not retrieve a list of all of NOC ICA certificates (ICACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one NOC ICA certificates (ICACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for following certificates	
ICACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_NOC_ICA (ICACs) command completed successfully	retrieve a list of all of NOC ICA certificates (ICACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one NOC ICA certificates (ICACs)	
GET_ALL_NOC_ICA (ICACs) command failed	does not retrieve a list of all of NOC ICA certificates (ICACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one NOC ICA certificates (ICACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REVOKED_NOC_ROOT (RCACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
RCACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REVOKED_NOC_ROOT (RCACs) command completed successfully	gets all revoked NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one revoked NOC root certificates (RCACs)	
GET_ALL_REVOKED_NOC_ROOT (RCACs) command failed	does not gets all revoked NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one revoked NOC root certificates (RCACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for following certificates	
RCACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REVOKED_NOC_ROOT (RCACs) command completed successfully	gets all revoked NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one revoked NOC root certificates (RCACs)	
GET_ALL_REVOKED_NOC_ROOT (RCACs) command failed	does not gets all revoked NOC root certificates (RCACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one revoked NOC root certificates (RCACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REVOKED_NOC_ICA (ICACs)	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
query works for following certificates	
ICACs	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REVOKED_NOC_ICA (ICACs) command completed successfully	gets all revoked NOC ica certificates (ICACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one revoked NOC ica certificates (ICACs)	
GET_ALL_REVOKED_NOC_ICA (ICACs) command failed	does not gets all revoked NOC ica certificates (ICACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one revoked NOC ica certificates (ICACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
query works for following certificates	
ICACs	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REVOKED_NOC_ICA (ICACs) command completed successfully	gets all revoked NOC ica certificates (ICACs)
ADD_NOC_ROOT (RCAC) command completed successfully	
there is at least one revoked NOC ica certificates (ICACs)	
GET_ALL_REVOKED_NOC_ICA (ICACs) command failed	does not gets all revoked NOC ica certificates (ICACs)
ADD_NOC_ROOT (RCAC) command failed	
there are not one revoked NOC ica certificates (ICACs)	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### PROPOSE_ADD_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROPOSE_ADD_ACCOUNT command completed successfully	proposes a new Account with the given address, public key and role
sufficient number of approvals is received	account added
insufficient number of approvals is received	account in a pending state
PROPOSE_ADD_ACCOUNT command failed	does not proposes a new Account with the given address, public key and role
approvals is not received	account not added
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
pub_key (Public Key)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
vid (Vendor ID )	optional(uint16)
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	MAX = 65535
pid_ranges (Product ID Ranges)	optional(array<uint16 range>)
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
the data stored in the array matches the expected format	
the data stored in the array does not exceed the permissible limits	
the list is displayed in ascending order	
     * Negative:	
empty value
value =< 0
string value format		
length > MAX	MAX = 65535
roles (Roles)	array<string>
     * Positive:	
support value	
Vendor	
TestHouse	
CertificationCenter	
Trustee	
NodeAdmin	
VendorAdmin	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
all array elements are of different types	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROPOSE_ADD_ACCOUNT command completed successfully	proposes a new Account with the given address, public key and role
sufficient number of approvals is received	account added
insufficient number of approvals is received	account in a pending state
PROPOSE_ADD_ACCOUNT command failed	does not proposes a new Account with the given address, public key and role
approvals is not received	account not added
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
pub_key (Public Key)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
vid (Vendor ID )	optional(uint16)
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
pid_ranges (Product ID Ranges)	optional(array<uint16 range>)
     * Positive:	
unique combination	
value > 0	
integer value format
nonexistent ID	
the data stored in the array matches the expected format	
the data stored in the array does not exceed the permissible limits	
the list is displayed in ascending order	
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 65535
roles (Roles)	array<string>
     * Positive:	
support value	
Vendor	
TestHouse	
CertificationCenter	
Trustee	
NodeAdmin	
VendorAdmin	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
all array elements are of different types	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### APPROVE_ADD_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
APPROVE_ADD_ACCOUNT command completed successfully	approves the proposed account
PROPOSE_ADD_ACCOUNT command completed successfully	
Number of required approvals greater than 2/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is active
Number of required approvals equal 2/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is active
Number of required approvals greater than 1/3 of Trustees for account role: Vendor	account is active
APPROVE_ADD_ACCOUNT command failed	does not approves the proposed account
PROPOSE_ADD_ACCOUNT command failed	
Number of required approvals less than 2/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is not active
Number of required approvals less than 1/3 of Trustees for account role: Vendor	account is not active
Number of required approvals equal 1/3 of Trustees for account role: Vendor	account is not active
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
APPROVE_ADD_ACCOUNT command completed successfully	approves the proposed account
PROPOSE_ADD_ACCOUNT command completed successfully	
Number of required approvals greater than 2/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is active
Number of required approvals equal 2/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is active
Number of required approvals greater than 1/3 of Trustees for account role: Vendor	account is active
APPROVE_ADD_ACCOUNT command failed	does not approves the proposed account
PROPOSE_ADD_ACCOUNT command failed	
Number of required approvals less than 2/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is not active
Number of required approvals less than 1/3 of Trustees for account role: Vendor	account is not active
Number of required approvals equal 1/3 of Trustees for account role: Vendor	account is not active
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### REJECT_ADD_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REJECT_ADD_ACCOUNT command completed successfully	rejects the proposed account
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
remove the proposal	
account has only proposer's approval and no rejects	
Number of required rejects greater than 1/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is reject
Number of required rejects greater than 2/3 of Trustees for account role: Vendor	account is reject
Number of required rejects equal 2/3 of Trustees for account role: Vendor	account is reject
REJECT_ADD_ACCOUNT command failed	does not rejects the proposed account
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
remove the proposal	
account has not only proposer's approval and no rejects	
account has only proposer's approval and rejects	
account has not only proposer's approval and rejects	
Number of required rejects equal 1/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is not reject
Number of required rejects less than 1/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is not reject
Number of required rejects less than 2/3 of Trustees for account role: Vendor	account is not reject
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
REJECT_ADD_ACCOUNT command completed successfully	rejects the proposed account
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
remove the proposal	
account has only proposer's approval and no rejects	
Number of required rejects greater than 1/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is reject
Number of required rejects greater than 2/3 of Trustees for account role: Vendor	account is reject
Number of required rejects equal 2/3 of Trustees for account role: Vendor	account is reject
REJECT_ADD_ACCOUNT command failed	does not rejects the proposed account
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
remove the proposal	
account has not only proposer's approval and no rejects	
account has only proposer's approval and rejects	
account has not only proposer's approval and rejects	
Number of required rejects equal 1/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is not reject
Number of required rejects less than 1/3 of Trustees for account roles: TestHouse, CertificationCenter, Trustee, NodeAdmin, VendorAdmin	account is not reject
Number of required rejects less than 2/3 of Trustees for account role: Vendor	account is not reject
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### PROPOSE_REVOKE_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROPOSE_REVOKE_ACCOUNT command completed successfully	proposes revocation of the Account with the given address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
sufficient number of approvals is received	account is revoke 
insufficient number of approvals is received	revocation in a pending state
PROPOSE_REVOKE_ACCOUNT command failed	does not proposes revocation of the Account with the given address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
approvals is not received	revocation rejected
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROPOSE_REVOKE_ACCOUNT command completed successfully	proposes revocation of the Account with the given address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
sufficient number of approvals is received	account is revoke 
insufficient number of approvals is received	revocation in a pending state
PROPOSE_REVOKE_ACCOUNT command failed	does not proposes revocation of the Account with the given address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
approvals is not received	revocation rejected
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### APPROVE_REVOKE_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
APPROVE_REVOKE_ACCOUNT command completed successfully	approves the proposed revocation of the account
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
Number of required approvals greater than 2/3 of Trustees	account is revoked
Number of required approvals equal 2/3 of Trustees	account is revoked
APPROVE_REVOKE_ACCOUNT command failed	does not approves the proposed revocation of the account
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
Number of required approvals less than 2/3 of Trustees	account is not revoked
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
APPROVE_REVOKE_ACCOUNT command completed successfully	approves the proposed revocation of the account
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
Number of required approvals greater than 2/3 of Trustees	account is revoked
Number of required approvals equal 2/3 of Trustees	account is revoked
APPROVE_REVOKE_ACCOUNT command failed	does not approves the proposed revocation of the account
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
Number of required approvals less than 2/3 of Trustees	account is not revoked
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (information/notes)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
time (proposal time)	optional(int64)
     * Positive:	
default value	current time by default
empty value	
integer value format
     * Negative:	
length > MAX	MAX = 9 223 372 036 854 775 807
### GET_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ACCOUNT command completed successfully	gets an accounts by the address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
there is at least one account	
GET_ACCOUNT command failed	does not gets an accounts by the address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
there are not one accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ACCOUNT command completed successfully	gets an accounts by the address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully	
there is at least one account	
GET_ACCOUNT command failed	does not gets an accounts by the address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
there are not one accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_PROPOSED_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
valid command result	
accounts by the address	
proposed but not approved accounts	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROPOSED_ACCOUNT command completed successfully	gets a proposed but not approved accounts by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_PROPOSED_ACCOUNT command failed	does not gets a proposed but not approved accounts by its address
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROPOSED_ACCOUNT command completed successfully	gets a proposed but not approved accounts by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_PROPOSED_ACCOUNT command failed	does not gets a proposed but not approved accounts by its address
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REJECTED_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REJECTED_ACCOUNT command completed successfully	gets a rejected accounts by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully, but account rejected 	
there is at least one rejected accounts	
GET_REJECTED_ACCOUNT command failed	does not gets a rejected accounts by its address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
there are not one rejected accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REJECTED_ACCOUNT command completed successfully	gets a rejected accounts by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully, but account rejected 	
there is at least one rejected accounts	
GET_REJECTED_ACCOUNT command failed	does not gets a rejected accounts by its address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
there are not one rejected accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_PROPOSED_ACCOUNT_TO_REVOKE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROPOSED_ACCOUNT_TO_REVOKE command completed successfully	gets a proposed but not approved accounts to be revoked by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_PROPOSED_ACCOUNT_TO_REVOKE command failed	does not gets a proposed but not approved accounts to be revoked by its address
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROPOSED_ACCOUNT_TO_REVOKE command completed successfully	gets a proposed but not approved accounts to be revoked by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_PROPOSED_ACCOUNT_TO_REVOKE command failed	does not gets a proposed but not approved accounts to be revoked by its address
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_REVOKED_ACCOUNT	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REVOKED_ACCOUNT command completed successfully	gets a revoked account by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_REVOKE_ACCOUNT command completed successfully	
there is at least one revoked account	
GET_REVOKED_ACCOUNT command failed	does not gets a revoked account by its address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_REVOKE_ACCOUNT  command failed	
there are not one revoked account	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REVOKED_ACCOUNT command completed successfully	gets a revoked account by its address
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_REVOKE_ACCOUNT command completed successfully	
there is at least one revoked account	
GET_REVOKED_ACCOUNT command failed	does not gets a revoked account by its address
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_REVOKE_ACCOUNT  command failed	
there are not one revoked account	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_ACCOUNTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_ACCOUNTS command completed successfully	gets all accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_REVOKE_ACCOUNT command completed successfully	
there is at least one account	
GET_ALL_ACCOUNTS command failed	does not gets all accounts
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_REVOKE_ACCOUNT  command failed	
there are not one account	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_ACCOUNTS command completed successfully	gets all accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_REVOKE_ACCOUNT command completed successfully	
there is at least one account	
GET_ALL_ACCOUNTS command failed	does not gets all accounts
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_REVOKE_ACCOUNT  command failed	
there are not one account	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_PROPOSED_ACCOUNTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROPOSED_ACCOUNTS command completed successfully	gets all proposed but not approved accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_ALL_PROPOSED_ACCOUNTS command failed	does not gets all proposed but not approved accounts
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROPOSED_ACCOUNTS command completed successfully	gets all proposed but not approved accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_ALL_PROPOSED_ACCOUNTS command failed	does not gets all proposed but not approved accounts
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REJECTED_ACCOUNTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REJECTED_ACCOUNTS command completed successfully	gets all rejected accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully, but account rejected 	
there is at least one rejected accounts	
GET_ALL_REJECTED_ACCOUNTS command failed	does not getsall rejected accounts
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
there are not one rejected accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REJECTED_ACCOUNTS command completed successfully	gets all rejected accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_ADD_ACCOUNT command completed successfully, but account rejected 	
there is at least one rejected accounts	
GET_ALL_REJECTED_ACCOUNTS command failed	does not getsall rejected accounts
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_ADD_ACCOUNT command failed	
there are not one rejected accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_PROPOSED_ACCOUNTS_TO_REVOKE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROPOSED_ACCOUNTS_TO_REVOKE command completed successfully	gets all proposed but not approved accounts to be revoked
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_ALL_PROPOSED_ACCOUNTS_TO_REVOKE command failed	does not gets all proposed but not approved accounts to be revoked
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROPOSED_ACCOUNTS_TO_REVOKE command completed successfully	gets all proposed but not approved accounts to be revoked
PROPOSE_ADD_ACCOUNT command completed successfully	
there is at least one proposed but not approved accounts	
GET_ALL_PROPOSED_ACCOUNTS_TO_REVOKE command failed	does not gets all proposed but not approved accounts to be revoked
PROPOSE_ADD_ACCOUNT command failed	
there are not one proposed but not approved accounts	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REVOKED_ACCOUNTS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REVOKED_ACCOUNTS command completed successfully	gets all revoked accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_REVOKE_ACCOUNT command completed successfully	
there is at least one revoked account	
GET_ALL_REVOKED_ACCOUNTS command failed	does not gets all revoked accounts
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_REVOKE_ACCOUNT  command failed	
there are not one revoked account	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REVOKED_ACCOUNTS command completed successfully	gets all revoked accounts
PROPOSE_ADD_ACCOUNT command completed successfully	
APPROVE_REVOKE_ACCOUNT command completed successfully	
there is at least one revoked account	
GET_ALL_REVOKED_ACCOUNTS command failed	does not gets all revoked accounts
PROPOSE_ADD_ACCOUNT command failed	
APPROVE_REVOKE_ACCOUNT  command failed	
there are not one revoked account	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### ADD_VALIDATOR_NODE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ADD_VALIDATOR_NODE command completed successfully	adds a new Validator node
ADD_VALIDATOR_NODE command failed	does not adds a new Validator node
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	
Parameters:	
pubkey (Public Key)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
moniker (Moniker)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
identity (Identity)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
website (Website)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
details (Details)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
ip (IP)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
node-id (Node ID)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
ADD_VALIDATOR_NODE command completed successfully	adds a new Validator node
ADD_VALIDATOR_NODE command failed	does not adds a new Validator node
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	
Parameters:	
pubkey (Public Key)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
moniker (Moniker)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
empty value	
identity (Identity)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
website (Website)	optional(string)
     * Positive:	
value exists	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
details (Details)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
ip (IP)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
node-id (Node ID)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### DISABLE_VALIDATOR_NODE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
DISABLE_VALIDATOR_NODE command completed successfully	disables the Validator node (removes from the validator set)
ADD_VALIDATOR_NODE command completed successfully	
there is at least one Validator node	
DISABLE_VALIDATOR_NODE command failed	does not disables the Validator node (removes from the validator set)
ADD_VALIDATOR_NODE command failed	
there is not a one Validator node	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	
owner	
not owner	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
DISABLE_VALIDATOR_NODE command completed successfully	disables the Validator node (removes from the validator set)
ADD_VALIDATOR_NODE command completed successfully	
there is at least one Validator node	
DISABLE_VALIDATOR_NODE command failed	does not disables the Validator node (removes from the validator set)
ADD_VALIDATOR_NODE command failed	
there is not a one Validator node	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	
owner	
not owner	
### PROPOSE_DISABLE_VALIDATOR_NODE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROPOSE_DISABLE_VALIDATOR_NODE command completed successfully	proposes disabling of the Validator node from the validator set
ADD_VALIDATOR_NODE command completed successfully	
there is at least one Validator node	
sufficient number of approvals is received	disable confirmed
insufficient number of approvals is received	disable in a pending state
PROPOSE_DISABLE_VALIDATOR_NODE command failed	does not proposes disabling of the Validator node from the validator set
ADD_VALIDATOR_NODE command failed	
there is not a one Validator node	
approvals is not received	disable rejected
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROPOSE_DISABLE_VALIDATOR_NODE command completed successfully	proposes disabling of the Validator node from the validator set
ADD_VALIDATOR_NODE command completed successfully	
there is at least one Validator node	
sufficient number of approvals is received	disable confirmed
insufficient number of approvals is received	disable in a pending state
PROPOSE_DISABLE_VALIDATOR_NODE command failed	does not proposes disabling of the Validator node from the validator set
ADD_VALIDATOR_NODE command failed	
there is not a one Validator node	
approvals is not received	disable rejected
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### APPROVE_DISABLE_VALIDATOR_NODE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
APPROVE_DISABLE_VALIDATOR_NODE command completed successfully	approves disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command completed successfully	
PROPOSE_DISABLE_VALIDATOR_NODE command completed successfully	
sufficient number of Trustees approve	validator node is disabled
APPROVE_DISABLE_VALIDATOR_NODE command failed	does not approves disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command failed	
PROPOSE_DISABLE_VALIDATOR_NODE command failed	
insufficient number of Trustees approve	validator node is not disabled
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
APPROVE_DISABLE_VALIDATOR_NODE command completed successfully	approves disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command completed successfully	
PROPOSE_DISABLE_VALIDATOR_NODE command completed successfully	
sufficient number of Trustees approve	validator node is disabled
APPROVE_DISABLE_VALIDATOR_NODE command failed	does not approves disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command failed	
PROPOSE_DISABLE_VALIDATOR_NODE command failed	
insufficient number of Trustees approve	validator node is not disabled
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### REJECT_DISABLE_VALIDATOR_NODE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REJECT_DISABLE_VALIDATOR_NODE command completed successfully	rejects disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command completed successfully	
PROPOSE_DISABLE_VALIDATOR_NODE command completed successfully	
remove the proposal	
disable validator proposal has only proposer's approval and no rejects	
number of rejects more than 1/3 of Trustees	validator node is reject
REJECT_DISABLE_VALIDATOR_NODE command failed	does not approves disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command failed	
PROPOSE_DISABLE_VALIDATOR_NODE command failed	
remove the proposal	
certificate has not proposer's approval	
certificate has only proposer's approval and rejects	
number of rejects less than 1/3 of Trustees	validator node is not reject
number of rejects equals 1/3 of Trustees	validator node is not reject
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
REJECT_DISABLE_VALIDATOR_NODE command completed successfully	rejects disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command completed successfully	
PROPOSE_DISABLE_VALIDATOR_NODE command completed successfully	
remove the proposal	
disable validator proposal has only proposer's approval and no rejects	
number of rejects more than 1/3 of Trustees	validator node is reject
REJECT_DISABLE_VALIDATOR_NODE command failed	does not approves disabling of the Validator node by a Trustee
ADD_VALIDATOR_NODE command failed	
PROPOSE_DISABLE_VALIDATOR_NODE command failed	
remove the proposal	
certificate has not proposer's approval	
certificate has only proposer's approval and rejects	
number of rejects less than 1/3 of Trustees	validator node is not reject
number of rejects equals 1/3 of Trustees	validator node is not reject
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
info (Information/Notes)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
### ENABLE_VALIDATOR_NODE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
ENABLE_VALIDATOR_NODE command completed successfully	enables the Validator node (returns to the validator set)
ADD_VALIDATOR_NODE command completed successfully	
DISABLE_VALIDATOR_NODE command completed successfully	
ENABLE_VALIDATOR_NODE command failed	does not enables the Validator node (returns to the validator set)ustee
ADD_VALIDATOR_NODE command failed	
DISABLE_VALIDATOR_NODE command failed	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	
owner	
not owner	error
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
ENABLE_VALIDATOR_NODE command completed successfully	enables the Validator node (returns to the validator set)
ADD_VALIDATOR_NODE command completed successfully	
DISABLE_VALIDATOR_NODE command completed successfully	
ENABLE_VALIDATOR_NODE command failed	does not enables the Validator node (returns to the validator set)ustee
ADD_VALIDATOR_NODE command failed	
DISABLE_VALIDATOR_NODE command failed	
Role (Who can send)	
Trustee	error
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	
owner	
not owner	error
### GET_VALIDATOR	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_VALIDATOR command completed successfully	gets a validator node
ADD_VALIDATOR_NODE command completed successfully	
there is at least one validator node	
GET_VALIDATOR command failed	does not gets a validator node
ADD_VALIDATOR_NODE command failed	
there is not a one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_VALIDATOR command completed successfully	gets a validator node
ADD_VALIDATOR_NODE command completed successfully	
there is at least one validator node	
GET_VALIDATOR command failed	does not gets a validator node
ADD_VALIDATOR_NODE command failed	
there is not a one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_VALIDATORS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_VALIDATORS command completed successfully	gets the list of all validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
there is at least one validator node	
there are only active stored validator nodes	
there are only jailed stored validator nodes	
there are both active and jailed stored validator nodes	all stored validator nodes (active and jailed) will be returned by default
GET_ALL_VALIDATORS command failed	does not gets the list of all validator nodes from the store
ADD_VALIDATOR_NODE command failed	
there is not a one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_VALIDATORS command completed successfully	gets the list of all validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
there is at least one validator node	
there are only active stored validator nodes	
there are only jailed stored validator nodes	
there are both active and jailed stored validator nodes	all stored validator nodes (active and jailed) will be returned by default
GET_ALL_VALIDATORS command failed	does not gets the list of all validator nodes from the store
ADD_VALIDATOR_NODE command failed	
there is not a one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_PROPOSED_DISABLE_VALIDATOR	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROPOSED_DISABLE_VALIDATOR command completed successfully	gets a proposed validator node
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
there is at least one proposed validator node	
GET_PROPOSED_DISABLE_VALIDATOR command failed	does not gets a proposed validator node
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
there is not a one proposed validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROPOSED_DISABLE_VALIDATOR command completed successfully	gets a proposed validator node
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
there is at least one proposed validator node	
GET_PROPOSED_DISABLE_VALIDATOR command failed	does not gets a proposed validator node
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
there is not a one proposed validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_PROPOSED_DISABLE_VALIDATORS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROPOSED_DISABLE_VALIDATORS command completed successfully	gets a the list of all proposed disable validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
there is at least one proposed validator node	
GET_ALL_PROPOSED_DISABLE_VALIDATORS command failed	does not gets a the list of all proposed disable validator nodes from the store
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
there is not a one proposed validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROPOSED_DISABLE_VALIDATORS command completed successfully	gets a the list of all proposed disable validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
there is at least one proposed validator node	
GET_ALL_PROPOSED_DISABLE_VALIDATORS command failed	does not gets a the list of all proposed disable validator nodes from the store
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
there is not a one proposed validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_REJECTED_DISABLE_VALIDATOR	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REJECTED_DISABLE_VALIDATOR command completed successfully	gets a rejected validator node
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
REJECTED_DISABLE_VALIDATOR command completed successfully	
there is at least one rejected validator node	
GET_REJECTED_DISABLE_VALIDATOR command failed	does not gets a rejected validator node
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
REJECTED_DISABLE_VALIDATOR command failed	
there are not one rejected validator nodes	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REJECTED_DISABLE_VALIDATOR command completed successfully	gets a rejected validator node
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
REJECTED_DISABLE_VALIDATOR command completed successfully	
there is at least one rejected validator node	
GET_REJECTED_DISABLE_VALIDATOR command failed	does not gets a rejected validator node
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
REJECTED_DISABLE_VALIDATOR command failed	
there are not one rejected validator nodes	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_REJECTED_DISABLE_VALIDATORS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REJECTED_DISABLE_VALIDATOR command completed successfully	gets the list of all rejected disable validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
REJECTED_DISABLE_VALIDATOR command completed successfully	
there is at least one rejected validator node	
GET_REJECTED_DISABLE_VALIDATOR command failed	does not gets the list of all rejected disable validator nodes from the store
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
REJECTED_DISABLE_VALIDATOR command failed	
there are not one rejected validator nodes	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REJECTED_DISABLE_VALIDATOR command completed successfully	gets the list of all rejected disable validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
REJECTED_DISABLE_VALIDATOR command completed successfully	
there is at least one rejected validator node	
GET_REJECTED_DISABLE_VALIDATOR command failed	does not gets the list of all rejected disable validator nodes from the store
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
REJECTED_DISABLE_VALIDATOR command failed	
there are not one rejected validator nodes	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_DISABLED_VALIDATOR	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_DISABLED_VALIDATOR command completed successfully	gets a disabled validator node
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
APPROVE_DISABLE_VALIDATOR_NODE command completed successfully	
there is at least one disabled validator node	
GET_REJECTED_DISABLE_VALIDATOR command failed	does not gets a disabled validator node
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
APPROVE_DISABLE_VALIDATOR_NODE command failed	
there are not one disabled validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_DISABLED_VALIDATOR command completed successfully	gets a disabled validator node
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
APPROVE_DISABLE_VALIDATOR_NODE command completed successfully	
there is at least one disabled validator node	
GET_REJECTED_DISABLE_VALIDATOR command failed	does not gets a disabled validator node
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
APPROVE_DISABLE_VALIDATOR_NODE command failed	
there are not one disabled validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_DISABLED_VALIDATORS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_DISABLED_VALIDATORS command completed successfully	gets a the list of all disabled validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
APPROVE_DISABLE_VALIDATOR_NODE command completed successfully	
there is at least one disabled validator node	
GET_ALL_DISABLED_VALIDATORS command failed	does not gets a the list of all disabled validator nodes from the store
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
APPROVE_DISABLE_VALIDATOR_NODE command failed	
there are not one disabled validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_DISABLED_VALIDATORS command completed successfully	gets a the list of all disabled validator nodes from the store
ADD_VALIDATOR_NODE command completed successfully	
PROPOSED_DISABLE_VALIDATOR command completed successfully	
APPROVE_DISABLE_VALIDATOR_NODE command completed successfully	
there is at least one disabled validator node	
GET_ALL_DISABLED_VALIDATORS command failed	does not gets a the list of all disabled validator nodes from the store
ADD_VALIDATOR_NODE command failed	
PROPOSED_DISABLE_VALIDATOR command failed	
APPROVE_DISABLE_VALIDATOR_NODE command failed	
there are not one disabled validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_LAST_VALIDATOR_POWER	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_LAST_VALIDATOR_POWER command completed successfully	gets a last validator node power
there is at least one validator node	
GET_LAST_VALIDATOR_POWER command failed	does not gets a last validator node power
there are not one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_LAST_VALIDATOR_POWER command completed successfully	gets a last validator node power
there is at least one validator node	
GET_LAST_VALIDATOR_POWER command failed	does not gets a last validator node power
there are not one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
address (Address)	string 
     * Positive:	
string matches the format	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
nonexistent value	
length > MAX	
### GET_ALL_LAST_VALIDATORS_POWER	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_LAST_VALIDATORS_POWER command completed successfully	gets the list of all last validator nodes power from the store
there is at least one validator node	
GET_ALL_LAST_VALIDATORS_POWER command failed	does not gets the list of all last validator nodes power from the store
there are not one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_LAST_VALIDATORS_POWER command completed successfully	gets the list of all last validator nodes power from the store
there is at least one validator node	
GET_ALL_LAST_VALIDATORS_POWER command failed	does not gets the list of all last validator nodes power from the store
there are not one validator node	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### PROPOSE_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
PROPOSE_UPGRADE command completed successfully	proposes an upgrade plan with the given name at the given height
number of  approvals greater than 2/3 of Trustees	upgrade approvals
upgrade proposal with the same name	
current upgrade proposal is out of date (when the current network height is greater than the proposed upgrade height)	
PROPOSE_UPGRADE command failed	does not proposes an upgrade plan with the given name at the given height
number of  approvals equals 2/3 of Trustees	upgrade not approvals
number of  approvals less than 2/3 of Trustees	upgrade not approvals
upgrade proposal with the same name	
current upgrade proposal is not out of date 	
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
current upgrade proposal is out of date	
current upgrade proposal is не out of date	error 
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
upgrade-height (Upgrade Height)	int64
     * Positive:	
value > 0	
integer value format
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 9 223 372 036 854 775 807
upgrade-info (Upgrade Info)	optional(string)
     * Positive:	
empty value	
text value format
value format	os/architecture
URL format	each URL include the corresponding checksum as checksum query parameter with the value in the format type:value
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
PROPOSE_UPGRADE command completed successfully	proposes an upgrade plan with the given name at the given height
number of  approvals greater than 2/3 of Trustees	upgrade approvals
upgrade proposal with the same name	
current upgrade proposal is out of date (when the current network height is greater than the proposed upgrade height)	
PROPOSE_UPGRADE command failed	does not proposes an upgrade plan with the given name at the given height
number of  approvals equals 2/3 of Trustees	upgrade not approvals
number of  approvals less than 2/3 of Trustees	upgrade not approvals
upgrade proposal with the same name	
current upgrade proposal is not out of date 	
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
current upgrade proposal is out of date	
current upgrade proposal is не out of date	error 
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
upgrade-height (Upgrade Height)	int64
     * Positive:	
value > 0	
integer value format
     * Negative:	
empty value	
value =< 0
string value format	
length > MAX	MAX = 9 223 372 036 854 775 807
upgrade-info (Upgrade Info)	optional(string)
     * Positive:	
empty value	
text value format
value format	os/architecture
URL format	each URL include the corresponding checksum as checksum query parameter with the value in the format type:value
MIN < length < MAX	
     * Negative:	
length > MAX	
сontains spaces or line breaks	
### APPROVE_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
APPROVE_UPGRADE command completed successfully	aproves the proposed upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
number of  approvals greater than 2/3 of Trustees	upgrade approvals
APPROVE_UPGRADE command failed	does not aproves the proposed upgrade plan with the given name
PROPOSE_UPGRADEcommand failed	
number of  approvals equals 2/3 of Trustees	upgrade not approvals
number of  approvals less than 2/3 of Trustees	upgrade not approvals
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
APPROVE_UPGRADE command completed successfully	aproves the proposed upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
number of  approvals greater than 2/3 of Trustees	upgrade approvals
APPROVE_UPGRADE command failed	does not aproves the proposed upgrade plan with the given name
PROPOSE_UPGRADEcommand failed	
number of  approvals equals 2/3 of Trustees	upgrade not approvals
number of  approvals less than 2/3 of Trustees	upgrade not approvals
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
### REJECT_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
REJECT_UPGRADE command completed successfully	rejects the proposed upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
remove the proposal	
proposed upgrade has only proposer's approval and no rejects	
number of rejects more than 1/3 of Trustees	upgrade rejects 
REJECT_UPGRADE command failed	does not rejects the proposed upgrade plan with the given name
PROPOSE_UPGRADE command failed	
remove the proposal	
proposed upgrade has not proposer's approval	
proposed upgrade has only proposer's approval and rejects	
number of rejects equals 1/3 of Trustees	upgrade not rejects 
number of rejects less than 1/3 of Trustees	upgrade not rejects 
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
REJECT_UPGRADE command completed successfully	rejects the proposed upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
remove the proposal	
proposed upgrade has only proposer's approval and no rejects	
number of rejects more than 1/3 of Trustees	upgrade rejects 
REJECT_UPGRADE command failed	does not rejects the proposed upgrade plan with the given name
PROPOSE_UPGRADE command failed	
remove the proposal	
proposed upgrade has not proposer's approval	
proposed upgrade has only proposer's approval and rejects	
number of rejects equals 1/3 of Trustees	upgrade not rejects 
number of rejects less than 1/3 of Trustees	upgrade not rejects 
Role (Who can send)	
Trustee	
Vendor 	error
VendorAdmin 	error
CertificationCenter 	error
NodeAdmin 	error
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
### GET_PROPOSED_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_PROPOSED_UPGRADE command completed successfully	gets the proposed upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
there is at least one proposed upgrade plan	
GET_PROPOSED_UPGRADE command failed	does not gets the proposed upgrade plan with the given name
PROPOSE_UPGRADE command failed	
there is not a one proposed upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_PROPOSED_UPGRADE command completed successfully	gets the proposed upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
there is at least one proposed upgrade plan	
GET_PROPOSED_UPGRADE command failed	does not gets the proposed upgrade plan with the given name
PROPOSE_UPGRADE command failed	
there is not a one proposed upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
### GET_APPROVED_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_APPROVED_UPGRADE command completed successfully	gets the approved upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
APPROVED_UPGRADE command completed successfully	
there is at least one approved upgrade plan	
GET_APPROVED_UPGRADE command failed	does not gets the approved upgrade plan with the given name
PROPOSE_UPGRADE command failed	
APPROVED_UPGRADE command failed	
there is not a one approved upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_APPROVED_UPGRADE command completed successfully	gets the approved upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
APPROVED_UPGRADE command completed successfully	
there is at least one approved upgrade plan	
GET_APPROVED_UPGRADE command failed	does not gets the approved upgrade plan with the given name
PROPOSE_UPGRADE command failed	
APPROVED_UPGRADE command failed	
there is not a one approved upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
### GET_REJECTED_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_REJECTED_UPGRADE command completed successfully	gets the rejected upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
REJECTED_UPGRADE command completed successfully	
there is at least one rejected upgrade plan	
GET_REJECTED_UPGRADE command failed	does not gets the rejected upgrade plan with the given name
PROPOSE_UPGRADE command failed	
REJECTED_UPGRADE command failed	
there is not a one rejected upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_REJECTED_UPGRADE command completed successfully	gets the rejected upgrade plan with the given name
PROPOSE_UPGRADE command completed successfully	
REJECTED_UPGRADE command completed successfully	
there is at least one rejected upgrade plan	
GET_REJECTED_UPGRADE command failed	does not gets the rejected upgrade plan with the given name
PROPOSE_UPGRADE command failed	
REJECTED_UPGRADE command failed	
there is not a one rejected upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
name (Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
### GET_ALL_PROPOSED_UPGRADES	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_PROPOSED_UPGRADES command completed successfully	gets all the proposed upgrade plans
PROPOSE_UPGRADE command completed successfully	
there is at least one proposed upgrade plans	
GET_ALL_PROPOSED_UPGRADES command failed	does not gets all the proposed upgrade plans
PROPOSE_UPGRADE command failed	
there is not a one proposed upgrade plans	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_PROPOSED_UPGRADES command completed successfully	gets all the proposed upgrade plans
PROPOSE_UPGRADE command completed successfully	
there is at least one proposed upgrade plans	
GET_ALL_PROPOSED_UPGRADES command failed	does not gets all the proposed upgrade plans
PROPOSE_UPGRADE command failed	
there is not a one proposed upgrade plans	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_APPROVED_UPGRADES	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_APPROVED_UPGRADES command completed successfully	gets all the approved upgrade plans
PROPOSE_UPGRADE command completed successfully	
APPROVED_UPGRADE command completed successfully	
there is at least one approved upgrade plan	
GET_ALL_APPROVED_UPGRADES command failed	does not gets all the approved upgrade plans
PROPOSE_UPGRADE command failed	
APPROVED_UPGRADE command failed	
there is not a one approved upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_APPROVED_UPGRADES command completed successfully	gets all the approved upgrade plans
PROPOSE_UPGRADE command completed successfully	
APPROVED_UPGRADE command completed successfully	
there is at least one approved upgrade plan	
GET_ALL_APPROVED_UPGRADES command failed	does not gets all the approved upgrade plans
PROPOSE_UPGRADE command failed	
APPROVED_UPGRADE command failed	
there is not a one approved upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_ALL_REJECTED_UPGRADES	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_ALL_REJECTED_UPGRADES command completed successfully	gets all the rejected upgrade plans
PROPOSE_UPGRADE command completed successfully	
REJECTED_UPGRADE command completed successfully	
there is at least one rejected upgrade plan	
GET_ALL_REJECTED_UPGRADES command failed	does not gets all the rejected upgrade plans
PROPOSE_UPGRADE command failed	
REJECTED_UPGRADE command failed	
there is not a one rejected upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_ALL_REJECTED_UPGRADES command completed successfully	gets all the rejected upgrade plans
PROPOSE_UPGRADE command completed successfully	
REJECTED_UPGRADE command completed successfully	
there is at least one rejected upgrade plan	
GET_ALL_REJECTED_UPGRADES command failed	does not gets all the rejected upgrade plans
PROPOSE_UPGRADE command failed	
REJECTED_UPGRADE command failed	
there is not a one rejected upgrade plan	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
count-total	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
limit 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value > 100	
offset 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page 	optional(uint)
     * Positive:	
value exists	
empty value	
     * Negative:	
value < 0	
page-key	optional(string)
     * Positive:	
empty value	
value exists	
     * Negative:	
length < MIN	
reverse	optional(bool)
     * Positive:	
empty value	
value state	
TRUE (-1)	
FALSE (0)	
     * Negative:	
value is not bool	
### GET_UPGRADE_PLAN	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_UPGRADE_PLAN command completed successfully	gets the currently scheduled upgrade plan, if it exists
currently scheduled upgrade plan exists	
GET_UPGRADE_PLAN command failed	does not gets the currently scheduled upgrade plan, if it exists
currently scheduled upgrade plan is not exists	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_UPGRADE_PLAN command completed successfully	gets the currently scheduled upgrade plan, if it exists
currently scheduled upgrade plan exists	
GET_UPGRADE_PLAN command failed	does not gets the currently scheduled upgrade plan, if it exists
currently scheduled upgrade plan is not exists	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
### GET_APPLIED_UPGRADE	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_APPLIED_UPGRADE command completed successfully	returns the header for the block at which the upgrade with the given name was applied, if it was previously executed on the chain
in the header for the block the upgrade with the given name was applied	
upgrade with the given name was previously executed on the chain	
GET_APPLIED_UPGRADE command failed	does not gets returns the header for the block at which the upgrade with the given name was applied, if it was previously executed on the chain
the upgrade with the given name was not applied in the header for the block	
upgrade with the given name was not previously executed on the chain	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
upgrade name (Upgrade Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_APPLIED_UPGRADE command completed successfully	returns the header for the block at which the upgrade with the given name was applied, if it was previously executed on the chain
in the header for the block the upgrade with the given name was applied	
upgrade with the given name was previously executed on the chain	
GET_APPLIED_UPGRADE command failed	does not gets returns the header for the block at which the upgrade with the given name was applied, if it was previously executed on the chain
the upgrade with the given name was not applied in the header for the block	
upgrade with the given name was not previously executed on the chain	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
upgrade name (Upgrade Name)	string 
     * Positive:	
value exists	
text value format
MIN < length < MAX	
     * Negative:	
empty value	
length > MAX	
### GET_MODULE_VERSIONS	
#### CLI command	
CLI command send	
Valid command	
command exists/relevant	
Invalid command	
access is denied to execute command	
incorrect command syntax	
Сommand result	
GET_MODULE_VERSIONS command completed successfully	gets a list of module names and their respective consensus versions.
module version is specified	
a specific module is specified	return only that module's information
specific module name not specified	returns list of module names
GET_MODULE_VERSIONS command failed	does not gets a list of module names and their respective consensus versions.
module version is not specified	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
module name (Module Name)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	
#### REST API 	
REST API command send	
Valid command	
correct HTTP method	
request is authorized	
uses valid credentials/role	
Invalid command	
incorrect request	
server side error	
Сommand result	
GET_MODULE_VERSIONS command completed successfully	gets a list of module names and their respective consensus versions.
module version is specified	
a specific module is specified	return only that module's information
specific module name not specified	returns list of module names
GET_MODULE_VERSIONS command failed	does not gets a list of module names and their respective consensus versions.
module version is not specified	
Role (Who can send)	
Trustee	
Vendor 	
VendorAdmin 	
CertificationCenter 	
NodeAdmin 	
Parameters:	
module name (Module Name)	optional(string)
     * Positive:	
empty value	
text value format
MIN < length < MAX	
     * Negative:	
length > MAX	

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
