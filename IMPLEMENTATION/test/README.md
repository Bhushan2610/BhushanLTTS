#include "unity.h"
#include <PROJECT.h>

#define PROJECT_NAME    "Game"
void setUp()
{
}
void tearDown()
{
}

void test_Project(void)
{
  TEST_ASSERT_EQUAL();
  TEST_ASSERT_EQUAL();
}
void test_Zero_One(void)
{
  TEST_ASSERT_EQUAL();
  TEST_ASSERT_EQUAL();
}
int main(void)
{
  UNITY_BEGIN();

  RUN_TEST(test_Zero_One);
  RUN_TEST(test_Negative);
  return UNITY_END();
}
