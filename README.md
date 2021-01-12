# RushPlate 
Templates for TypeScript, React and Redux projects that help you write your code faster.
_____
This VS Code extension includes templates for TypeScript, React and Redux projects. Templates are easy-to-memorize character sequences that expand into boilerplate code such as class or property definition. Templates help you write code faster. 


## Features

### Two Ways to Expand a Template

**RushPlate** allows you to quickly expand a template. If you know the template name, just type it and press **Space**. 

![](media/template_space.gif "Template space")

You can also choose the required item from the IntelliSence list and press **Enter**.


### Context-dependent Templates 

**RushPlate** analyzes code and expands different templates depending on the context. For example, **RushPlate** can create the following code for the "c" template: 

  1. A class, if you expand the template in a file root. 
  2. A constructor, if you expand the template inside a class.
  3. A constant, if you expand the template inside a constructor. 

![](media/template_context.gif "Template context")


### Dependent Namespace Declaration

**RushPlate** adds dependent imports to the top of a file, where other imports are located. It also checks if similar modules are already exist and adds only modules that are not declared in the file.

![](media/template_namespace_declaration.gif "Template namespace declaration")


### Linked Identifiers

If a template contains linked identifiers used several times in code, you can quickly change identifiers’ name in one link after the template expansion and **RushPlate** will change text  in other links.
**RushPlate** also keeps links active constantly. You can remove the caret from links, for example, move the caret to another file, and then, go back and continue your change. 

![](media/template_links.gif "Template links")


### Different Prefixes for the Same Templates

**RushPlate** can expand templates using short combinations such as "c" (to add a class, constructor, or constant), "rc" (to add a React component), " rpc" (to add a React Pure component), and others. If you prefer to use a more understandable and standardized syntax, you can expand the same templates using the following mnemonics: "class", "react component", "react pure component".


![](media/template_prefixes.gif "Template prefixes")


## Usage

Type a template name, for example **c**, and press **Space** or choose the "c" item from  IntelliSense and press **Enter**. **RushPlate** creates a class and suggests its name. Press **Enter** to apply this suggestion or change this name. 

The screencast below shows "c" and ""arf" template expansions:

![](media/template_usage.gif "Template usage")


## Code Templates

The following tables list all available templates for TypeScript, React and Redux:

### TypeScript Templates

#### Import/Export 

| Template  | Description  | 
|---|---|
| **imd**, **id**  | Imports a default module. | 
| **imp**, **ip**  | Imports a module part. | 
| **ima**  | Imports a whole module. | 
| **exd**  | Exports a default declaration. |
| **exp**  | Exports a current module part.  |
| **exmp**  | Exports another module part.   |
| **exf**  | Exports a function. |
| **exdf**  | Exports a default function. |
| **exc**  | Exports a class. |
| **excc**  | Exports a class with a constructor. |

#### Members 

| Template  | Description  | 
|---|---|
| **c**  | Creates a class or constructor or declares a constant depending on the caret's current position. |
| **cc**  | Creates a class with a constructor. |
| **cci**  | Adds interface implementer. |
| **cce**  | Creates a class with inheritance. 
| **e**  | Adds an enum.
| **p**  | Creates a procedure.
| **f**  | Creates a function.
| **arp**  | Creates an arrow procedure.
| **arf**  | Creates an arrow function.
| **asf**  | Creates an async function.
| **asarf**  | Creates an async arrow function.
| **prop**  | Creates a property.
| **rprop**  | Creates a read-only property.
| **g**, **get**  | Creates a property get declaration.
| **s**, **set**  | Creates a property set declaration.

#### Conditionals & Control Statements

 Template  | Description  | 
|---|---|
| **forof**  | Creates a for-of statement. | 
| **forin**  | Creates a for-in statement. | 
| **w**,**while**  | Creates a while statement. | 
| **if**  | Creates an if conditional.
| **ife**  | Creates an if-else conditional. |
| **sw**, **switch**  | Creates a switch conditional. |
| **ca**, **case**  | Creates a case statement. |
| **tc**, **trycatch**  | Creates a try/catch block. |
| **tcf**, **trycatchfinally**  | Creates a try/catch/finally block. |
| **tf**, **tryfinally**  | Creates a try/finally block. |
| **te**, **throwerror**  | Creates a new error statement. |
| **prom**  | Creates a promise declaration. | 
| **r**  | Creates a return statement. | 
| **ru** | Creates a return undefined statement. | 
| **rt**  | Creates a return true statement.
| **rf**  | Creates a return false statement. |

#### Declarations

 Template  | Description  | 
|---|---|
| **v**, **let**  | Creates a variable declaration. |
| **vn**  | Creates a field/variable/parameter declaration of the number type. |
| **vs** |Creates a field/variable/ parameter declaration of the string type. |
| **vb** |Creates a field/variable/ parameter declaration of the boolean type. |
| **va** | Creates a field/variable/parameter declaration of any type. |
| **vt**  | Creates a field/variable/parameter declaration of the specified type. |

### TypeScript React Templates

 Template  | Description  | 
|---|---|
| **imr**, **react import all**  | Imports a React module. |
| **imrn**, **react import namespace**  | Imports a React namespace. |
|**imrr**, **react router import**  | Imports a router from React-router. | 
|**imrrd**, **react router dom import** | Imports a router from the React-router-dom.. | 
|**imc**, **react component import** | Imports a Component. | 
|**impc**, **react pure component import** | Imports a PureComponent. | 
|**imfc**, **react function component import** | Imports a FunctionComponent. | 
|**imus**, **react usestate import** | Imports a FunctionComponent. | 
|**imse**, **react useeffect import** | Imports as useState and useEffect. | 
|**rc**, **react component** | Declares as React Component. | 
|**rcs**, **react component with state** | Declares a React component with a state. | 
|**rpc**, **react pure component** | Declares a React PureCompoment. |
|**rpcs**, **react pure component with state** | Declares a React PureCompoment with a state. |
|**rfc**, **react function component** | Declares a React Function component. |
|**rafc**, **react arrow function component**|Declares a React Arrow Function component. |
|**rsfc**, **,react stateless function component**|Declares a React Stateless Function component. |
|**c**, **react component constructor** |Declares a React component constructor. |
|**cwm**, **react componentWillMount** |Declares a componentWillMount method. |
|**cdm**, **react componentDidMount** |Declares a componentDidMount method. |
|**cwum**, **react componentWillUnmount** |Declares a componentWillUnmount method. |
|**scu**, **react shouldComponentUpdate**|Declares a shouldComponentUpdate method. |
|**bnd**, **react bind** |Declares a bind method call. |
|**ss**, **react setState** |Declares a setState method call. |
|**us**, **react useState** |Declares a useState method call. |
|**ue**, **react useEffect** |Declares a useEffect method call. |

### TypeScript Redux Templates

 Template  | Description  | 
|---|---|
| **imrd**, **redux import**| Imports all from Redux. |
| **imcon**, **redux connect import**| Imports connect from Redux. |
| **rrc**, **redux component**| Creates a Redux component. |
| **rrcd**, **redux component with dispatch**| Creates a Redux component with dispatch. |
| **rrcdp**, **redux component with own props**| Creates a Redux component with dispatch and own properties. |
| **mstp**, **redux map state**| Creates a mapStateToProps function. |
| **mstpp**, **redux map state and props** | Creates a mapStateToProps function with component properties. |
| **mdtp**, **redux map dispatch**| Creates a mapDispatchToProps function. |
| **mdtpb**, **redux map dispatch with bind**| Creates a mapDispatchToProps function with bindActionCreators. |
| **rrcon**, **redux connect**| Creates a React Redux connect. |
| **rrfc**, **redux function component**| Creates a Redux function component. |
| **rrfc**, **redux function component**| Creates a Redux function component. |

### TypeScript Action Templates

 Template  | Description  | 
|---|---|
| **acr**, **redux actions create**| Creates an action creator. |
| **bacr**, **redux actions bind**| Binds an action creator. |


### TypeScript Reducer Templates

 Template  | Description  | 
|---|---|
| **rd**, **redux reducer**| Creates a reducer declaration. |
| **crd**, **redux combine reducers**| Creates combineReducers. |


### TypeScript Middleware Templates

 Template  | Description  | 
|---|---|
| **mw**, **middleware function**| Creates a Middleware function. |
| **mw**, **middleware crash logger**| Creates a crash logger middleware. |
| **cst**, **redux create store** | Creates a Redux store. |
| **cstmw**, **redux create store with middleware** | Creates a Redux store with middleware.
|

### TypeScript Console Templates

 Template  | Description  | 
|---|---|
| **clm**, **console log**| Creates a console log message. |
| **clt**, **console time**| Creates a console log time. |
| **clinf**, **console info** | Creates a console log info. |
| **cler**, **console error** | Creates a console log error.
| **clex**, **console exception** | Creates a console log exception.

