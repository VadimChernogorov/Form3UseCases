Ещё не готово, т.к. не успел написать превращение чаров в верхний регистр и разделение их пробелами.
Но написал схему.
После главного If напишу один или несколько extentionов в else.

    using System;
    using System.Collections.Generic;
    using System.ComponentModel;
    using System.Data;
    using System.Drawing;
    using System.Linq;
    using System.Text;
    using System.Threading.Tasks;
    using System.Windows.Forms;
    using ClassLibraryCsharp;
    //using UpperText;
    //using Probel;

namespace WindowsFormsApplicationCsharp
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            string outer = textBox1.Text;
            if (checkBox1.Text != "")
            {
                if(checkBox1.Checked)
                {
                    textreverse reverse = new textreverse();
                    outer = reverse.ReversT(outer);
                }

                if (checkBox2.Checked)
                {
                    // uppertext upper = new uppertext();
                    // outer = upper.setToUpper(outer)
                }

                if (checkBox3.Checked)
                {
                    // textspace space = new textspace();
                    // outer = space.setSpace(outer)
                }
                textBox1.Text = outer;
            }
           

        }
    }
}
