
### 1. 클래스 정의

먼저, `Animal` 클래스를 정의합니다. 이것은 모든 동물의 기본 설계도입니다.

```javascript
class Animal {
    constructor(name, species, age) {
        this.name = name;
        this.species = species;
        this.age = age;
    }

    eat() {
        console.log(`${this.name} is eating.`);
    }

    sleep() {
        console.log(`${this.name} is sleeping.`);
    }

    makeSound() {
        console.log(`${this.name} is making a sound.`);
    }
}
```

### 2. 객체 생성

`Animal` 클래스를 사용하여 구체적인 동물 객체를 생성합니다.

```javascript
const simba = new Animal('Simba', 'Lion', 5);
const polly = new Animal('Polly', 'Parrot', 2);

simba.eat();    // Simba is eating.
polly.sleep();  // Polly is sleeping.
```

### 3. 상속

동물의 종류별로 더 구체적인 행동을 추가하기 위해 상속을 사용합니다. 예를 들어, 포유류 클래스와 조류 클래스를 만듭니다.

```javascript
class Mammal extends Animal {
    nurse() {
        console.log(`${this.name} is nursing its young.`);
    }

    makeSound() {
        console.log(`${this.name} is roaring.`);
    }
}

class Bird extends Animal {
    fly() {
        console.log(`${this.name} is flying.`);
    }

    makeSound() {
        console.log(`${this.name} is chirping.`);
    }
}
```

### 4. 상속받은 클래스의 객체 생성

`Mammal` 클래스와 `Bird` 클래스를 사용하여 구체적인 동물 객체를 생성합니다.

```javascript
const mufasa = new Mammal('Mufasa', 'Lion', 8);
const tweety = new Bird('Tweety', 'Canary', 1);

mufasa.eat();         // Mufasa is eating.
mufasa.nurse();       // Mufasa is nursing its young.
mufasa.makeSound();   // Mufasa is roaring.

tweety.sleep();       // Tweety is sleeping.
tweety.fly();         // Tweety is flying.
tweety.makeSound();   // Tweety is chirping.
```

### 5. 다형성

다형성을 통해 `makeSound` 메서드를 다양한 방식으로 구현합니다. 각 클래스는 `makeSound` 메서드를 자신만의 방식으로 재정의(오버라이딩)합니다.

```javascript
function animalSound(animal) {
    animal.makeSound();
}

animalSound(simba);   // Simba is making a sound.
animalSound(mufasa);  // Mufasa is roaring.
animalSound(tweety);  // Tweety is chirping.
```

