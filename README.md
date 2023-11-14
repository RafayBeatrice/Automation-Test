# Automation-Test



## **Choose Yes or No Button**

/// <reference types= "cypress"/>

describe('Validate Checkbox & Radio Button', function () {
 
  
  it( 'Test Yes and Check', function () {
    cy.visit('https://demo.guru99.com/test/ajax.html')
    cy.get('input[type="radio"]').check('Yes')
    cy.get('#buttoncheck').click()
  })

  it('Test No and Check', function() {
    cy.visit('https://demo.guru99.com/test/ajax.html')
    cy.get('input[type="radio"]').check('No')
    cy.get('#buttoncheck').click()
  })

  it('Test Yes, Check and reset together', function(){
    cy.visit('https://demo.guru99.com/test/ajax.html')
    cy.get('input[type="radio"]').check('Yes')
    cy.get('#buttoncheck').click()
    cy.get('[type="reset"]').click()

})
it('Test No, Check and reset together', function(){
  cy.visit('https://demo.guru99.com/test/ajax.html')
  cy.get('input[type="radio"]').check('No')
  cy.get('#buttoncheck').click()
  cy.get('[type="reset"]').click()

})
  
})

## **How to delete a Customer**

// <reference types= "cypress"/>

describe('Validate Checkbox & Radio Button', function () {
 
  
  it( 'Test Yes and Check', function () {
    cy.visit('https://demo.guru99.com/test/delete_customer.php')
    cy.get(':nth-child(2) > :nth-child(2) > input').type('1111')
    cy.get('[type="submit"]').click()
    cy.on('window:confirm', (AcceptConfirm) => 
    
    expect(AcceptConfirm).to.contains('Do you really want to delete this Customer?')
    )}
  )}
)



## **How to Upload File**


/// <reference types= "cypress"/>

describe('Test Upload File ', function () {
  it('Upload File', function(){
    cy.once('uncaught:exception', () => false);
    
  
    cy.visit('https://demo.guru99.com/test/upload/')

    const myFile = '4213602.png'
    cy.get('#uploadfile_0').attachFile(myFile)
    cy.get('inplut[type="checkbox"]').check()
    cy.get('#submitbutton').click()
  })
})
## **Check the Radio and Checkbox**

/// <reference types= "cypress"/>

describe('Validate Checkbox & Radio Button', function () {
 
/*
 it( 'Validate checkbox', function () {

    cy.visit('https://demo.guru99.com/test/radio.html')
  //check all Boxes
    cy.get('input[type="checkbox"]').check()
  //Uncheck all Boxes
    cy.get('input[type="checkbox"]').uncheck()
  //Check one specific checkbox
    cy.get('input[type="checkbox"]').check('checkbox2');
})
*/
it('Validate Radio Button', function(){

   cy.visit('https://demo.guru99.com/test/radio.html')
//Check first Radio Button
   cy.get('input[type="radio"]').first().check()
//Check one specific Radio Button
   cy.get('input[type="radio"]').check('Option 3')

})
})



## **How to log in account**



describe('On OrangeHRM', () => {

      it('I can login', () => {
        cy.visit('https://opensource-demo.orangehrmlive.com/web/index.php/auth/login');
        cy.get(':nth-child(2) > .oxd-input-group > :nth-child(2) > .oxd-input').type('Admin');
        cy.get(':nth-child(3) > .oxd-input-group > :nth-child(2) > .oxd-input').type('admin123');
        cy.get('.oxd-button').click();
    })
})

***************************************************************
## **How to purchase something**

describe('On DemoBlaze', () => {


    
        // it('Purchase', () => {
        //    cy.visit('https://www.demoblaze.com/');
        //    cy.get(':nth-child(1) > .card > .card-block > .card-title > .hrefch').click();
        //     cy.get('.col-sm-12 > .btn').click();
        //     cy.get('#cartur').click();
        //     cy.get('.col-lg-1 > .btn').click();
        //     cy.get('#name').type('test1');
        //     cy.get('#country').type('Romania');
        //     cy.get('#city').type('Brasov');
        //     cy.get('#card').type('123456789');
        //     cy.get('#month').type('3');
        //     cy.get('#year').type('2040');
        //     cy.get('#orderModal > .modal-dialog > .modal-content > .modal-footer > .btn-primary').click();
        //     cy.get('.confirm').click();
        // })

*************************

## **How to view "About us**

        // it('About us', () => {
        //     cy.visit('https://www.demoblaze.com/');
        //     cy.get(':nth-child(3) > .nav-link').click();
        // })
       
    })

## **How to buy products with an account/ How to sign up / How to login**

describe('On Store', () => {

    it('Purchase', () =>{
    
        cy.visit('https://automationteststore.com/');
        cy.get('#block_frame_bestsellers_1771 > .thumbnails > :nth-child(3) > .thumbnail > :nth-child(1) > img').click();
        cy.get('#option347767').click();
        cy.get('#product_quantity').click();
        cy.get('#product_quantity').clear();
        cy.get('#product_quantity').type('3');
        cy.get('.cart').click();
        cy.get('#cart_checkout1').click();
        cy.get('#accountFrm > fieldset > .btn').click();
        cy.get('#AccountFrm_firstname').type('Maria');
        cy.get('#AccountFrm_lastname').type('Popescu');
        cy.get('#AccountFrm_email').type('mariapopescu@d2311anmm.com');
        cy.get('#AccountFrm_address_1').type('Str.Mihai Eminescu');
        cy.get('#AccountFrm_city').type('Brasov');
        cy.get('#AccountFrm_zone_id').select('3515');
        cy.get('#AccountFrm_postcode').type('341241');
        cy.get('#AccountFrm_country_id').select('1');
        cy.get('#AccountFrm_loginname').type('Beatrice4332111');
        cy.get('#AccountFrm_password').type('1234');
        cy.get('#AccountFrm_confirm').type('1234');
        cy.get('#AccountFrm_newsletter0').click();
        cy.get('#AccountFrm_agree').click();
        cy.get('.col-md-2 > .btn').click();
        cy.get('#AccountFrm_zone_id').select('26');
        cy.get('#AccountFrm_password').type('1234');
        cy.get('#AccountFrm_confirm').type('1234');
        cy.get('.col-md-2 > .btn').click();
        cy.get('#checkout_btn').click();
        cy.get('#customer_menu_top > :nth-child(1) > .top > .menu_text').click();
        cy.get('#customer_menu_top > :nth-child(1) > .top > .menu_text').click();
        cy.get('.side_account_list > :nth-child(10) > a').click();
        cy.get('.logo > img').click();
    cy.get('[href="https://automationteststore.com/index.php?rt=product/category&path=68"]').click();
    cy.get(':nth-child(2) > .mt10 > a').click();
    cy.get(':nth-child(3) > .fixed_wrapper > .fixed > .prdocutname').click();
    cy.get('#option350').select('775');
    cy.get('#product_quantity').clear();
    cy.get('#product_quantity').type('2');
    cy.get('.cart').click();
    cy.get('.logo > img').click();
    cy.get('#block_frame_featured_1769 > .thumbnails > :nth-child(1) > .fixed_wrapper > .fixed > .prdocutname').click();
    cy.get('#product_quantity').clear();
    cy.get('#product_quantity').type('100');
    cy.get('.cart').click();
    cy.get('.logo > img').click();
    cy.get('.nextArrow').click().should('be.visible');
    cy.get('.nextArrow').click();
    cy.get('.prevArrow').click();
    cy.get('#brandcarousal > :nth-child(7)').click();
    cy.get('#customer_menu_top > li > a').click();
    cy.get('#loginFrm_loginname').type('tttt');
    cy.get('#loginFrm_password').type('tttt');
    cy.get('#loginFrm > fieldset > .btn').click();
    cy.get('.block_7 > .nav > .dropdown > .dropdown-toggle').click();
    cy.get('#cart_quantity121cf270a9f0b2596b85990ba40feaeccad').clear();
    cy.get('#cart_quantity121cf270a9f0b2596b85990ba40feaeccad').type('10');
    cy.get('#cart_update').click();
    cy.get('#estimate_country').select('2');
    cy.get('#estimate_country_zones').select('34');
    cy.get('#estimate_postcode').type('320034');
    cy.get(':nth-child(2) > .input-group > .input-group-btn > .btn').click();
    cy.get('#cart_checkout2').click();
    cy.get('#loginFrm_loginname').type('Beatrice4332111');
    cy.get('#loginFrm_password').type('1234');
    cy.get('#loginFrm > fieldset > .btn').click();
    cy.get('#checkout_btn').click();
    })
})

