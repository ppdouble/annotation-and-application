---

title: "" 
---

- Annotation: 
  - *to provide extra metadata about your program* 
  - *no other effect on execution of the annotated code*

- **@Override**
  - *compile-time checking*
  - *checking whether you actually are overriding a method from parent class*

```Java
public final class CartItem {
    private final int id;
    private final String name;
    private double cost;

    private CartItem(int id, String name, double cost) {
        this.id = id;
        this.name = Objects.requireNonNull(name);
        this.cost = cost;
    }

    public boolean equals(CartItem other) {
        if (this == other) {
            return true;
        }
        return this.id == other.id && this.name.equals(other.name) && this.cost == other.cost;
    }

    @Override
    public int hashCode() {
        return Objects.hash(id, name, cost);
    }

    public String getName() {
        return name;
    }

    public double getCost() {
        return cost;
    }

    public static void main(String[] args) {
        CartItem book1 = new CartItem(17, "Hitchhiker's Guide to the Galaxy", 7.14);
        CartItem book2 = new CartItem(17, "Hitchhiker's Guide to the Galaxy", 7.14);

        Set<CartItem> items = new HashSet<>();
        items.add(book1);
        items.add(book2);

        System.out.println(items.size());
    }
}
```
