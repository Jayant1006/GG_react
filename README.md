# GG_react

Prank APP
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <title>Document</title>
</head>

<body>
    <div id="app">

    </div>
    <script type="text/babel">
        class App extends React.Component {
            state = {
                name: 'Jayant',
                age: 20
            }
            handleClick(e) {
                //target : HTML which the function is passed as a event 
            }
            handleMouseOver(e) {
                console.log(e.target, e.pageX, e.pageY);
            }
            handleCopy(e) {
                alert("Ab toh sudhar ja BSDK!");
            }
            render() {
                return (
                    <div className="app-content">
                        <h1>Hey {this.state.name}</h1>
                        <p>My age is {this.state.age}</p>
                        <button onClick={this.handleClick}>Click Me </button>
                        <button onMouseOver={this.handleMouseOver}>Hover Me</button>
                        <p onCopy={this.handleCopy}>What we think,We become</p>
                    </div>
                )
            }
        }
        ReactDOM.render(<App />, document.getElementById('app'));
    </script>

</body>


</html>
