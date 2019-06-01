# Comment Models



## Header

```c++
////////////////////////////////////////////////////////////////////////////////////////////
///
/// @file [filename]
/// 
/// @author [your name]
/// @date [date of creation]
///
/// [comment]
///
/// @license MIT
///
////////////////////////////////////////////////////////////////////////////////////////////

```



## Class and Structs

```c++
///
/// @class [class name]
/// @brief [brief description]
/// [detailed description]
/// 
/// @author [your name]
/// @date [date of creation]
///
class ClassName 
{
    ...
}

///
/// @struct [struct name]
/// @brief [brief description]
/// [detailed description]
/// 
/// @author [your name]
/// @date [date of creation]
///
struct StructName 
{
    ...
}
```



## Methods and Functions

```c++
///
/// @brief [brief description]
///
/// [detailed description]
///
/// @param[in] [name of input parameter] [its description]
/// @param[out] [name of output parameter] [its description]
/// @param[in,out] [name of output parameter] [its description]
/// @return [information about return value]
/// @sa [see also section]
/// @note [any note about the function you might have]
/// @warning [any warning if necessary]
///
int function(int i, int &o, int &io) const
{
    ...
}
```



## Unions and Enums

```c++
///
/// @enum  [name]
/// @brief [brief description]
///
/// [detailed description]
///
enum class SomeEnum 
{
    ONE, 	///< [Explain ONE]
    TWO, 	///< [Explain TWO]
    THREE 	///< [Explain THREE]
}

///
/// @union [name]
/// @brief [brief description]
///
/// [detailed description]
///
union SomeUnion 
{
    int MEDIUM, 	///< [Explain MEDIUM]
    double LARGE, 	///< [Explain LARGE]
    char TINY		///< [Explain TINY]
}
```



## Templates

All template classes, structs, functions and methods are just the regular ones related to their comments. The only change is the use of *tparam* to specify the template parameters. The syntax is just like the regular *param*.



```c++
///
/// @class [class name]
/// @brief [brief description]
/// [detailed description]
///
/// @tparam [name of template input parameter] [its description]
/// 
/// @author [your name]
/// @date [date of creation]
///
template<typename T>
class TClassName 
{
    ...
}

///
/// @brief [brief description]
///
/// [detailed description]
/// 
/// @tparam [name of template input parameter] [its description]
/// @param[in] [name of input parameter] [its description]
/// @param[out] [name of output parameter] [its description]
/// @param[in,out] [name of output parameter] [its description]
/// @return [information about return value]
/// @sa [see also section]
/// @note [any note about the function you might have]
/// @warning [any warning if necessary]
///
template<typename T>
int tfunction(int i, int &o, int &io) const
{
    ...
}
```



## Alias

```c++
///
/// [Brief alias explanation]
///
typedef SomeType TypedefAlias;

///
/// [Brief alias explanation]
///
using UsingAlias = SomeOtherType;

```



## Other

Other useful comments to use:



### Design by Contract

Used in functions to document contracts.

```c++
...
/// @invariant 	[description of invariant]
/// @pre 		[description of pre-condition]		
/// @post 		[description of post-condition]	
...
```

### Extra documentation

```c++
/// @attention 		[Explain a detail that requires the user full attetion]
/// @note 			[Relevant notes. Note vital, but useful]
/// @bug			[If there is a important bug related to the feature. Doc it.]
/// @deprecated		[A brief please-don't-use-it message]
/// @exception  	<user-defined-exception-object> [exception description]
/// @throw 			<exception-object> [exception description]
/// @remarks		[Something worth mention]
/// @warning		[Dangerous behavior must be communicated]
```

### Groups

Grouping is a powerful semantic tool.

```c++
/// @addtogroup <label> 
/// @{
///
... //[content forming a group]
/// @}
```

