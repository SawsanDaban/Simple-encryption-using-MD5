package encryption;

public class EncryptMD5 {


    public static byte[] digest(byte[] input) {
        MessageDigest md;
        try {
            md = MessageDigest.getInstance("MD5");
        } catch (NoSuchAlgorithmException e) {
            throw new IllegalArgumentException(e);
        }
        byte[] result = md.digest(input);
        return result;
    }

    public static String bytesToHex(byte[] bytes) {
        StringBuilder sb = new StringBuilder();
        for (byte b : bytes) {
            sb.append(String.format("%02x", b));
        }
        return sb.toString();
    }
    
    
    public static void main(String[] args) {
        
        Scanner input = new Scanner(System.in);
        System.out.println("Enter a text: ");
        String text = input.next();
        
        byte[] md5InBytes = data.digest(text.getBytes(UTF_8));
        String textHex = data.bytesToHex(md5InBytes);
        
        System.out.println("Text before encryption: "+ text);
        
        System.out.println("Text after encryption: "+ textHex);
    }



}

