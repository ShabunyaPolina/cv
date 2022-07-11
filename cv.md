# Shabunya Polina
## Junior Developer
### *Contacts:*

**Phone:** 8029-821-02-14

**E-mail:** shabunya.polina@mail.ru

**Telegram:** @PolinaShabunya

[LinkedIn](https://www.linkedin.com/in/polina-shabunya-2648b7243/)

[GitHub](https://github.com/ShabunyaPolina)

---

### *About me:*

I’m a third-year student of FAMCS BSU with good academic performance and big ambitions

I started learning programming after entering university. Then I began to actively study Java myself, as well as in courses from one of the Belarusian IT companies. I am also interested in algorithmic and mathematical logic. Every day I practice writing code, developing university and personal projects. I strive to learn new programming languages and development tools, deepen knowledge on Java, explore new possibilities of the language and frameworks.

---

### *Skills and Proficiency:*
#### *Programming tools:*
* C++ (Qt)
* Java
* Assembly
* Git, GitHub
* Linux
* Microsoft Visual Studio, CLion, IntelliJ IDEA, VS Code

#### *Extra skills:*
* OOP
* Algorithms and data structures
* Mathematics

---

### *Languages:*
* English (B1)
* Russian (native)
* Belarusian (advanced)

---

### *Education:*
1. Lyceum №1 (2017-2019) 

   Minsk, Belarus

   Physical and mathematical direction. (Gold medal)
   
2. Belarusian State University, Faculty of Applied Mathematics and Informatics (2020 - Present)

   Minsk, Belarus
   
   Specialty - computer science

---
   
### *Code example:*
**Dijkstra's algorithm on C++:**
```
std::vector<std::vector<std::pair<long long, int>>> g;
std::vector<long long> dist;

void DoDijkstra() {
    std::vector<bool> processed(n, false);
    std::priority_queue<std::pair<long long, int>, std::vector<std::pair<long long, int>>, std::greater<>> q;

    q.push(std::make_pair(0, 0));

    while (!q.empty()) {
        std::pair<long long, int> e1 = q.top();
        q.pop();

        if (processed[e1.second]) continue;

        processed[e1.second] = true;
        dist[e1.second] = e1.first;

        for (auto &e2 : g[e1.second]) {
            if (!processed[e2.second] && e1.first + e2.first < dist[e2.second])
                q.push(std::make_pair(e1.first + e2.first, e2.second));
        }
    }
}
```
