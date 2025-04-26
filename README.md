# Spring Data JPA - Spring Data JPA

This repository contains source code examples to support my course Spring Data JPA and Hibernate Beginner to Guru

## Connect with Spring Framework Guru
* Spring Framework Guru [Blog](https://springframework.guru/)
* Subscribe to Spring Framework Guru on [YouTube](https://www.youtube.com/channel/UCrXb8NaMPQCQkT8yMP_hSkw)
* Like Spring Framework Guru on [Facebook](https://www.facebook.com/springframeworkguru/)
* Follow Spring Framework Guru on [Twitter](https://twitter.com/spring_guru)
* Connect with John Thompson on [LinkedIn](http://www.linkedin.com/in/springguru)


```

public interface BookRepository extends JpaRepository<Book, Long> {
  Book readByTitle(String title);

    @Nullable
    Book getByTitle(@Nullable String title);
-----------
package-infro.java >> this will enable nullapi within the package
@org.springframework.lang.NonNullApi
package guru.springframework.jdbc.repositories;
------------
  @Test
    void testEmptyResultException() {

        assertThrows(EmptyResultDataAccessException.class, () -> {
            Book book = bookRepository.readByTitle("foobar4");
        });
    }

```