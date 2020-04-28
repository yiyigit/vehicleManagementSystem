Vehicle Management System
INFO5100 Fall 2019 Final Project

## Assignment: making swing application as interface
CUI = character user interface (interact with character)
**GUI = graphical user interface (button/ text fields)**

make swing application steps:
1.create a container (where you dump all the ui)
2.create components 
3.set a layout to container
4.add components to the container
5.create listeners (event listener)
6.attach listeners to components
7.make the container visible

```java
import java.swing.JFrame
	JFrame frame = new JFrame();

	JButton button = new JButton(“Click Me”);
	JButton close = new JButton(“close”);

	FlowLayout fl = new FlowLayout();
						//add into end in flow layout eg.GridLayout

	Container con = frame.getContentPane();
	con.setLayout(fl);
	con.add(button);
	con.add(close);

	ActionEvent ae = new ActionEvent();
	button.addActionListener((ae)—> changeBackground(frame));

	frame.setSize(400,400);
	frame.setVisible(true);

static void changeBackground(JFrame jf){
	Color c = jf. getContentPane().getBackground();
	if (c == Color.RED){
		jf. getContentPane().setBackground(Color.Blue)
	} else{
		jf. getContentPane(). setBackground(Color.Red)
		}

}

if in a static function, calling static function and static class

public abstract class BaseFrame extends JFrame{
	private JLable
	private JTextField firstNumber, secondNumber;
	private JComboBox
	private JButton


}
```

