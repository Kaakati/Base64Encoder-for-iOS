## Base64Encoder for iOS [Objetive-C & Swift 2.0]
Convert to Base64 on iOS


#### Usage on Swift 2.0 for UIImage
<b>How to Convert UIImage to Base64 on Swift 2.0?</b>
<p>After you make the bridging-header on swift and #import "Base64Convertor.h"</p>

    let theImage : UIImage = UIImage(named:"image-name")
    var imageData = UIImageJPEGRepresentation(theImage, 1)
    var base64String = Base64Convertor.encodeBase64WithData(imageData)
    print("\(base64String)")

#### Available Methods
    +(NSString *)encodeBase64WithString:(NSString *)strData;
    +(NSString *)encodeBase64WithData:(NSData *)objData;
    +(NSData *)base64DataFromString: (NSString *)string;
