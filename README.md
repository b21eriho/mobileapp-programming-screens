# Report

Firstly, a secondary activity was created. On this secondary activity a text-view was made, constrained and given a place-holder text.
On the primary activity a button was made and given a button-listener that upon being clicked creates an intent with it's own activity -- as the
Context -- and the class form of the secondary activity. After this the button-listener adds an extra and starts an activity of that intent.
In the secondary activity's constructor it loads the extra and takes it as the new text for the title.

Below the code for creating the intent and starting an activity as well as screenshots of both activity's

```
private void onButtonClicked(){
    Intent intent = new Intent(this, SecondActivity.class);
    intent.putExtra("TITLE", "App Title");
    startActivity(intent);
}
```

![](First.png)
![](Second.png)
