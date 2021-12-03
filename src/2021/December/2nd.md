# 2021/12/2 (THU)

<div class="date_jumper">
  <a class="link_wrapper" href="./1st.md"><div class="button">go to the previous day</div></a>
  <a class="link_wrapper" href="./3rd.md"><div class="button">go to the next day</div></a>
</div>

## Univ.
### courses
#### *Programming Methodologies*
- Design Pattern
  - Command Pattern: extract complex requirements as Objects
  - Iterator Pattern: Commonly provided as Languages' basic functionality

#### *OS*
- Condition Variable
  - wait, signal
- DeadLock
- Dining Philosopher

#### *Pattern Information Processing*
- SVM

### homework
#### *Programming Methodologies*
```Java
public class Heater {
  public void turnOn() {
    System.out.println("Heater is on.");
  }
  public void turnOff() {
    System.out.println("Heater is off.");
  }
}

class HeaterOnCommand implements Command {
  private Heater aHeater;
  public HeaterOnCommand(Heater h) {
    this.aHeater = h;
  }
  public void execute() {
    aHeater.turnOn();
  }
}

class HeaterOffCommand implements Command {
  private Heater aHeater;
  public HeaterOnCommand(Heater h) {
    this.aHeater = h;
  }
  public void execute() {
    aHeater.turnOff();
  }
}
```

#### *OS*
- quiz

#### *Pattern Information Processing*
- exercise

## Other Activities
### Reading papers, articles, books, codes
- read [Visual Studio Codeで言語ごとにインデントの設定をしたい](https://ja.stackoverflow.com/questions/34014/visual-studio-codeで言語ごとにインデントの設定をしたい)
- read [TeXでソースコードをVSCode風に出力](https://zenn.dev/kyaon/articles/68867e2657e605)


## Memo, Feelings, Thoughts
- indentation setting  
  e.g. on `setting.json`,  
  ```json
  {
    "[markdown]": {
      "editor.tabSize": 2,
    },
  }
  ```
