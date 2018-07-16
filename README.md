```CSharp
 T? StringToType<T>(string data) where T : struct   
    {  
        if (string.IsNullOrEmpty(data)) 
        {
            return null; 
        }
        return (T)Convert.ChangeType(data,typeof(T)); 
    }
```
use T? and where T:struct, so can return null.  
if not null than return T's type value  
