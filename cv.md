# Kate Shpakovskaya
![img]()

## Contact information:
**Location:** Minsk,  Belarus  
**Phone:** +375445440657  
**E-mail:** <kate.shpakovskaya02@gmail.com>  
**Telegram:** [@shpakusua](https://t.me/shpakusua)  
**Discord rsschool:** Shpakusya(@shpakusya) 
## About me
I am studying at BSUIR as a marketing-programmer.
I like to solve non-standard tasks, I always learn something interesting and discover new opportunities for myself.
I have good communication skills and know how to work in a team.  
Always focus on achieving the most effective result in my work
## Skills
* C++
* Java (basic of JavaEE: RMI, CORBA, EJB, JSF)
* HTML
* CSS
* JS (basics)
* Git, GitHub
* VS, VS Code, Intellij IDEA, Eclipse
* MySQL
## Code example
```
@WebServlet("/phone")
public class PhoneServlet extends HttpServlet {
    @EJB
    PhoneServiceImpl phoneService;
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp)
            throws IOException {
        resp.setContentType("text/html");
        PrintWriter out = resp.getWriter();
        try {
            Vector<String> phones = phoneService.getPhones();
            for (int i = 0; i < 10; i++) {
                String[] arr = phones.get(i).split("");
                phones.set(i, arr[0] + "-" + arr[1] + arr[2] + "-" + arr[3] + arr[4] + "-" + arr[5] + arr[6]);
            }
            Collections.sort(phones);
            out.write(phones.toString());
        } catch (NumberFormatException e) {
            out.write("Error!");
        }
    }
}
```
## Education
* BSUIR
* HTML, CSS at [Code-basics](https://ru.code-basics.com/)
* JS manual on [learn.javascript.ru](https://learn.javascript.ru/)

## Languages
* Eng - C1 in online test EF Set [certificate](https://www.efset.org/cert/oAr9fD)
* Russian - Native
* Belarussian - Native