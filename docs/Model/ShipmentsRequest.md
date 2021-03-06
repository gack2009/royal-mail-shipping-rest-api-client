# ShipmentsRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**shipmentType** | **string** | Specifies whether the shipment being created is a standard delivery service or a returns service. Accepted values are ‘Delivery’ and ‘Return’. Please note that this field is not case sensitive. | 
**service** | [**\RoyalMail\Shipping\Rest\Api\models\Service**](Service.md) |  | 
**bfpoCode** | **string** | For HM Forces (BFPO) Service Type only when the Service Format is not International Flat, International Letter or International Packet. For the list of permissible values, please go to API Shipping V2 page on the Royal Mail API (Developer) Portal and refer to API Shipping Reference Data. | [optional] 
**shippingDate** | **string** | This is the date that the item will be physically sent (in the format YYYY-MM-DD). This may be up to 28 days in the future. Please note that for returns a Shipping date must be provided. | [optional] 
**items** | [**\RoyalMail\Shipping\Rest\Api\models\ShipmentRequestItemInternational[]**](ShipmentRequestItemInternational.md) |  | [optional] 
**recipientContact** | [**\RoyalMail\Shipping\Rest\Api\models\Contact**](Contact.md) |  | 
**recipientAddress** | [**\RoyalMail\Shipping\Rest\Api\models\Address**](Address.md) |  | 
**senderReference** | **string** | This field allows the user to supply their own reference number. Where supported (e.g. Tracked Returns) this number will appear on the label. | [optional] 
**departmentReference** | **string** | This is the department reference code that customers can define in OBA. | [optional] 
**customerReference** | **string** | This field allows customers to supply a reference that applies to multiple shipments and is included to mirror the functionality offered by the Customer Reference field in OBA, whereby a reference can be associated to a group of items. For references that apply to a single shipment, the senderReference field should be used. **Warning** Misuse of this field may result in incorrect billing. | [optional] 
**safePlace** | **string** | For Tracked non-signature service offerings only; this field allows a string that gives details of the recipient&#x27;s designated safeplace (e.g. “inside the porch”). | [optional] 
**internationalInfo** | **object** |  | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

