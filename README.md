 T? StringToType<T>(string data) where T : struct 
    {
        if (string.IsNullOrEmpty(data)) 
        {
            return null; 
        }
        return (T)Convert.ChangeType(data,typeof(T)); 
    }
