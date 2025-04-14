# React Interview questions

In a React component, how would you conditionally render a
'Login' button if the user is logged out, and a 'Logout'
button if they're logged in?

Solution

function AuthButton() {
const [isLoggedIn, setIsLoggedIn] = useState(false);

if (isLoggedIn) {
return <button onClick={() => setIsLoggedIn(false)}>Logout</button>;

}

return

<button onClick={() => setIsLoggedIn(true)}>Login

</button>;
}
