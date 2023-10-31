


@JsonValue 어노테이션을 사용하면 된다. 



```kotlin
enum class Role(val value: String, val description: String) {  
    SYSTEM("system", "시스템 설정"),  
    USER("user", "사용자"),  
    ASSISTANT("assistant", "ai 응답자"),  
    FUNCTION("function", "함수 설정");  
  
    @JsonValue  
    fun value(): String {  
        return value  
    }  
}
```



- 참고 
	 <https://www.baeldung.com/jackson-annotations#5-jsonvalue>


