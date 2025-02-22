import javax.swing.*;
import java.awt.*;

public class CircleDrawing extends JPanel {
    @Override
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        g.setColor(Color.BLUE); // Set circle color
        g.fillOval(50, 50, 100, 100); // Draw a filled circle (x, y, width, height)
    }

    public static void main(String[] args) {
        JFrame frame = new JFrame("Circle Drawing");
        CircleDrawing panel = new CircleDrawing();
        
        frame.add(panel);
        frame.setSize(400, 400);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setVisible(true);
    }
}
