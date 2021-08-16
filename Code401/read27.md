# <Login /> and <Auth />

## Review, Research, and Discussion

**1. Why is the Context API useful?**
    *The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.*

**2. Can a component outside of a provider get its context?**
    *To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext .*
**3. What are some common use cases for using the Context API?**
*Theming — Pass down app themei18n — Pass down translation messagesAuthentication — Pass down current authenticated user.*

**4. Describe Context Hell**
    *The React Context hell is the nasty code you get taking advantage of the React Context API.*


## Vocabulary Terms

* **global state**: a global state is a set of local states which are all concurrent with each other, a global state in the time domain is also a global state in the causal domain; if two states occur simultaneously, then they cannot have any cause-effect relationship.

* **global context:** is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a `theme` prop in order to style the Button component: class App extends React

* **provider:** The Provider component is what makes the state available to all children components no matter how deeply nested they are.

* **consumer:** The Consumer component allows a React component to subscribe to the context changes. The component makes the data available using a render prop.

## Preparation Materials

### what is role based access control?
* Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
* In computer systems security, role-based access control (RBAC) or role-based security is an approach to restricting system access to authorized users. ... The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments.
* Role-based access control (RBAC), also known as role-based security, is a mechanism that restricts system access. ... One role-based access control example is a set of permissions that allow users to read, edit, or delete articles in a writing application.

### BENEFITS OF RBAC:
* **Reducing administrative work and IT support** With RBAC, you can reduce the need for paperwork and password changes when an employee is hired or changes their role. Instead, you can use RBAC to add and switch roles quickly and implement them globally across operating systems, platforms and applications. It also reduces the potential for error when assigning user permissions.

* **Maximizing operational efficiency** RBAC offers a streamlined approach that is logical in definition. Instead of trying to administer lower-level access control, all the roles can be aligned with the organizational structure of the business and users can do their jobs more efficiently and autonomously.

* **Improving compliance** All organizations are subject to federal, state and local regulations. With an RBAC system in place, companies can more easily meet statutory and regulatory requirements for privacy and confidentiality as IT departments and executives have the ability to manage how data is being accessed and used. This is especially significant for health care and financial institutions, which manage lots of sensitive data such as PHI and PCI data.

## react-cookies component:
* Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them. To set or remove the cookies, we are going to use a third-party dependency of react-cookie.

* react-cookie provides a component that you wrap around your root component. This sets a cookies object, and allows us to start using cookies anywhere within this component. ... Import the component with import { CookiesProvider } from 'react-cookie'; . App.js. Now, within App.

