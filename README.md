Realizar a busca de um produto.
// Generated by Selenium IDE
const { Builder, By, Key, until } = require('selenium-webdriver')
const assert = require('assert')

describe('login_busca_produto', function() {
  this.timeout(30000)
  let driver
  let vars
  beforeEach(async function() {
    driver = await new Builder().forBrowser('chrome').build()
    vars = {}
  })
  afterEach(async function() {
    await driver.quit();
  })
  it('login_busca_produto', async function() {
    await driver.get("https://advantageonlineshopping.com/#/")
    await driver.manage().window().setRect({ width: 1004, height: 708 })
    await driver.findElement(By.id("menuUser")).sendKeys("Claudinei")
    await driver.findElement(By.name("password")).sendKeys("mANE@1980")
    await driver.findElement(By.id("menuUserSVGPath")).click()
    await driver.findElement(By.name("username")).click()
    await driver.findElement(By.name("password")).click()
    await driver.findElement(By.id("sign_in_btn")).click()
    await driver.findElement(By.id("speakersTxt")).click()
    await driver.findElement(By.linkText("HOME")).click()
    await driver.findElement(By.id("tabletsImg")).click()
    await driver.findElement(By.linkText("HOME")).click()
    await driver.findElement(By.id("laptopsTxt")).click()
    await driver.findElement(By.linkText("HOME")).click()
    {
      const element = await driver.findElement(By.id("miceImg"))
      await driver.actions({ bridge: true }).moveToElement(element).clickAndHold().perform()
    }
    {
      const element = await driver.findElement(By.id("miceTxt"))
      await driver.actions({ bridge: true }).moveToElement(element).release().perform()
    }
    await driver.findElement(By.id("miceImg")).click()
    await driver.findElement(By.linkText("HOME")).click()
    await driver.findElement(By.id("headphonesImg")).click()
    await driver.findElement(By.id("83")).click()
    await driver.findElement(By.linkText("HOME")).click()
    await driver.findElement(By.id("miceImg")).click()
    await driver.findElement(By.id("29")).click()
    await driver.findElement(By.linkText("HOME")).click()
    {
      const element = await driver.findElement(By.linkText("HOME"))
      await driver.actions({ bridge: true }).moveToElement(element).perform()
    }
    await driver.findElement(By.css("#img-special-offer img")).click()
    await driver.findElement(By.id("speakersImg")).click()
    await driver.findElement(By.id("25")).click()
    await driver.findElement(By.linkText("HOME")).click()
  })
})
