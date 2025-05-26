# Symmetric-
Program:

import java.security.SecureRandom:

import javax.crypto.KeyGenerator;

import javax.crypto.SecretKey;

import javax.xml.bind.DatatypeConverter;

public class symmetric

{

public static final String AES= "AES":

public static SecretKey createAESKey()

throws Exception

SecureRandom securerandom new SecureRandom();

KeyGenerator keygenerator KeyGenerator.getInstance(AES);

keygenerator.init(256, securerandom);

SecretKey key keygenerator.generateKey();

return key:

public static void main(String args[])

throws Exception

SecretKey Symmetrickey createAESKey();

System.out.println("Output");

System.out.print("The Symmetric Key is:"+

DatatypeConverter.printl HexBinary(Symmetrickey.getEncoded
