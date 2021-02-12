# Base64
Simple base64 conversion header only library in C++

Made it for myself for personal use, if you are looking for a high performance library for production, look elsewhere. I outlined ways to increase speed, made it so I can have quick access to base64 conversions for testing.

# Usage
You can do conversions by two ways, by the namespace Base64:: or by declaring the Base64 class

If you are going to do alot of conversions its best to declare the class so only 1 allocation of the encoding array and decoding hash-map is done

You can also use the B64::ToBase64(std::string) and B64::FromBase64(std::string) to perform the operation from a single function but the tables are allocated each function call so it is best to use the single functions when calling it only or twice
