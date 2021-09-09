The onClick prop on the built-in DOM <button> component tells React to set up a click event listener.
When the button is clicked, React will call the onClick event handler that is defined in Square’s render() method.
This event handler calls this.props.onClick(). The Square’s onClick prop was specified by the Board.
Since the Board passed onClick={() => this.handleClick(i)} to Square, the Square calls this.handleClick(i) when clicked.
We have not defined the handleClick() method yet, so our code crashes. If you click a square now, you should see a red error screen saying something like “this.handleClick is not a function”.
