## Base64Encoder for iOS [Objetice-C & Swift 2.0]
Convert to Base64 on iOS

#### Usage on Swift 2.0 for UIImage
After you make the bridging-header on swift and #import "Base64Convertor.h"

    let theImage : UIImage = UIImage(named:"image-name")
    var imageData = UIImageJPEGRepresentation(theImage, 1)
    var base64String = Base64Convertor.encodeBase64WithData(imageData)
    print("\(base64String)")

#### Available Methods
    +(NSString *)encodeBase64WithString:(NSString *)strData;
    +(NSString *)encodeBase64WithData:(NSData *)objData;
    +(NSData *)base64DataFromString: (NSString *)string;
