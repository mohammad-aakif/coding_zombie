# coding_zombie
coding
#include <GL/glut.h> // OpenGL Utility Toolkit

void display() {
    glClear(GL_COLOR_BUFFER_BIT);
    glColor3f(1.0, 1.0, 1.0); // Set color to white

    // Define vertices (you can adjust these)
    glBegin(GL_LINES);
    glVertex2f(-0.5, -0.5); // Vertex 1
    glVertex2f(0.5, -0.5);  // Vertex 2
    glVertex2f(0.5, -0.5);  // Vertex 2
    glVertex2f(0.0, 0.5);   // Vertex 3
    glVertex2f(0.0, 0.5);   // Vertex 3
    glVertex2f(-0.5, -0.5); // Vertex 1
    glEnd();

    glFlush();
}

int main(int argc, char** argv) {
    glutInit(&argc, argv);
    glutCreateWindow("Mustang Wireframe");
    glutDisplayFunc(display);
    glutMainLoop();
    return 0;
}
