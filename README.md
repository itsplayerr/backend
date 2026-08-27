PULSE TAG Backend Made By (player)

import json
import random
import requests
from flask import, jsonify requests

class GameInfo:
    def  init  (self):
        self.Titleid: str = "18AF6E"
        self.SecretKey: str = "CK9FRMOU9BM676F97OWOTIXN3NXZX96O6IQR6M47KQAGGT6DUN"
        self.ApiKey: str = "3IK64SPD19D8Q39JS1THJZPK6KK86M41KJ31GGX4FZDJSRPUWT"
        self.DiscordWebhook: str = "https://discord.com/api/webhooks/1491575366328782968/6ShzQ2OMrZ4AM3FR3kO4QQd1YLWUXtFLYp03ERIAH4ouaZZeZdge0a1HPwEK-6tm6m46"

def get_auth_headers(self)
return ("content type" : "application/json", "x SecretKey": self.SecretKey)


settings - GameInfo()
app-flask(__name__)


def return_function_json(data, funcname, funcparam()): 
    user_id - data["FunctionParameter"]["CallerEntityProfile"]["Lineage"]
        "titlePlayerAccountId"
    ]
    
     response - requests.post(
        url- ("https://{setting.titleId}").playfabapi.com/server/ExecuteCloudScript",
        json {
            "PlayFabId": user_id",
            "FunctionName": funcname,
            "FunctionParameter": funcparam,
        },
        headers.setting.get_auth_headers(),
     )

     if response.status_code -- 200:
        return  (
            jsonify(()), response.status_code

        )
    else:
        return  jsonify(()), response.status_code


,app.route("/", methoods-| "POST", "GET"|)
def main():
    return """"
        <html>
            <heac>
                <link href-"https://fonts.googleapis.com/css2family-inter:ugh/100:sea:
            <head>
            <body style "font.family: 'inter', sams-serif>
                <hi style-"color: red: font size: 10pxi">
                    luckily none of this will work for you skidder
                  </hi> 
              </body>
          </html>
       """
    app.route("/api/PlayFabAuthentcation", methoods ("POST|", "GFI"|)
    def luckys_PlayFabAuth():



        if request.content type ! "application/json":
            return jsonify(( 
                "BanMessage": "Your account has been banned"
                "BanExepirationTime": (time) 
                ]}, 400

           pluh - request.get_json()

           app_id = pluh.get('AppId')

           app_version - pluh.get('AppVersion')

           nonce - pluh.get('Nonce')  

           oculus_id - pluh.get('Oculus')

           platform - pluh.get('Platform')

           CustomIdNewFR - + "OCULUS{oculus_id}"

           login_req - requests.post(
            url = "https://(setting.TitleId.playfabapi.com/Server/LoginWithServerCustomID",
            json - (
                "ServerCustomId": CustomIdNewFR.
                "CreateAccount": True

                },
                headers = {
                    "x-SecretKey": settings.SecretKey,
                    "Content Type": "application/json"

                }}

                if login_req.status_code -- 200:

                    rjson - login req.json().get("data") if Makes It So That You Dont Have To Get "data The Whole Time."

                    session_ticket - rjson.get("SessionTicket")

                    entity_token - i json.get("EntityToken").get("EntityToken")
[
  {
    "Action": "*",
    "Effect": "Allow",
    "Resource": "*--*",
    "Principal": {
      "ChildOf": {
        "EntityType": "namespace",
        "EntityId": "E72F99713710450"
      }
    },
    "Comment": "The default allow title in namespace full access",
    "Condition": {
      "CallingEntityType": "title"
    }
  },
  {
    "Action": "*",
    "Effect": "Allow",
    "Resource": "pfrn:data--*!*/Profile/*",
    "Principal": "[SELF]",
    "Comment": "The default allow profile self access",
    "Condition": null
  },
  {
    "Action": "*",
    "Effect": "Allow",
    "Resource": "pfrn:data--*!*/Profile/*",
    "Principal": {
      "ChildOf": {
        "EntityType": "*"
      }
    },
    "Comment": "The default allow profile child access",
    "Condition": null
  },
  {
    "Action": "Write",
    "Effect": "Deny",
    "Resource": "pfrn:data--*!*/Profile/Statistics/*",
    "Principal": "*",
    "Comment": "Only title can edit user statistics",
    "Condition": {
      "CallingEntityType": "title_player_account"
    }
  },
  {
    "Action": "Write",
    "Effect": "Deny",
    "Resource": "pfrn:data--*!*/Profile/Statistics/*",
    "Principal": "*",
    "Comment": "Only title can edit user statistics",
    "Condition": {
      "CallingEntityType": "character"
    }
  },
  {
    "Action": "Write",
    "Effect": "Deny",
    "Resource": "pfrn:data--*!*/Profile/Statistics/*",
    "Principal": "*",
    "Comment": "Only title can edit user statistics",
    "Condition": {
      "CallingEntityType": "master_player_account"
    }
  },
  {
    "Action": "Write",
    "Effect": "Deny",
    "Resource": "pfrn:data--group!*/Profile/Statistics/*",
    "Principal": {
      "MemberOf": {
        "RoleId": "*"
      }
    },
    "Comment": "Only title can edit group statistics",
    "Condition": null
  },
  {
    "Action": "LobbyServerFull",
    "Effect": "Allow",
    "Resource": "pfrn:data--game_server!*/Lobby/Server/*",
    "Principal": {
      "ChildOf": {
        "EntityType": "title",
        "EntityId": "18AF6E"
      }
    },
    "Comment": "The Default allow title full Lobby server functionality",
    "Condition": {
      "CallingEntityType": "game_server"
    }
  },
  {
    "Action": "Read",
    "Effect": "Allow",
    "Resource": "*--*",
    "Principal": {
      "ChildOf": {
        "EntityType": "namespace",
        "EntityId": "E72F99713710450"
      }
    },
    "Comment": "The default allow game_server in namespace full access",
    "Condition": {
      "CallingEntityType": "game_server"
    }
  },
  {
    "Action": "Write",
    "Effect": "Allow",
    "Resource": "*--*",
    "Principal": {
      "ChildOf": {
        "EntityType": "namespace",
        "EntityId": "E72F99713710450"
      }
    },
    "Comment": "The default allow game_server in namespace full access",
    "Condition": {
      "CallingEntityType": "game_server"
    }
  },
  {
    "Action": "Create",
    "Effect": "Allow",
    "Resource": "*--*",
    "Principal": {
      "ChildOf": {
        "EntityType": "namespace",
        "EntityId": "E72F99713710450"
      }
    },
    "Comment": "The default allow game_server in namespace full access",
    "Condition": {
      "CallingEntityType": "game_server"
    }
  }
]

handlers.validatePlayerAction = function(args, context) {
    var knownCheatTools = [
        "LemonLoader",
        "LemonInstaller",
        "MelonLoader",
        "MelonInstaller",
        "DevX",
        "CheatEngine",
        "ArtMoney",
        "Xenos",
        "Extreme Injector",
        "Sourcetree",
        "DLL Injector",
        "Process Hacker",
        "Winject"
        // Add more patchers here
    ];

    if (!r["UserInfo"]["CustomIdInfo"]["CustomId"].startsWith("OCULUS")) {


        var c = {
        "content": null,
        "embeds": [
            {
             "title": "user's custom id doesn't start with OCULUS.",
            "color": 11339013,
            "fields": [
                {
                "name": "User Information",
                "value": "```diff\n+ CustomId: " + r["UserInfo"]["CustomIdInfo"]["CustomId"] + "\n- UserId: " + currentPlayerId + "\n```"
                }
            ]
         }
        ],
         "attachments": []
      }

        tasrequestSystem(web, "POST", c)

        EasierBanning(currentPlayerId, 8, "INVALID ID")
        EasierDeletePlayer(currentPlayerId)=


    }

     var url = "https://discord.com/api/webhooks/1325242249084403842/x19GnYgp7LcLcRMCWee-7Y024h_qXhJeaqpdxHyaZrYdLMPnAFkuYf2lFkKj3qnsl00R"
    var method = "post";
    var contentType = "application/json";
    var headers = {};
    var responseString = http.request(url, method, JSON.stringify(contentBody), contentType, headers);
  }
}
// Triggered automatically when a Photon room is first created
handlers.RoomCreated = function (args) {
    log.debug("Room Created - Game: " + args.GameId + " MaxPlayers: " + args.CreateOptions.MaxPlayers);
};

// Triggered automatically when a player joins a Photon room
handlers.RoomJoined = function (args) {
    log.debug("Room Joined - Game: " + args.GameId + " PlayFabId: " + args.UserId);
};

// Triggered automatically when a player leaves a Photon room
handlers.RoomLeft = function (args) {
    log.debug("Room Left - Game: " + args.GameId + " PlayFabId: " + args.UserId);
};

// Triggered automatically when a Photon room closes
// Note: currentPlayerId is undefined in this function
handlers.RoomClosed = function (args) {
    log.debug("Room Closed - Game: " + args.GameId);
};

// Triggered automatically when a Photon room game property is updated.
// Note: currentPlayerId is undefined in this function
handlers.RoomPropertyUpdated = function (args) {
    log.debug("Room Property Updated - Game: " + args.GameId);
};

// Triggered by calling "OpRaiseEvent" on the Photon client. The "args.Data" property is 
// set to the value of the "customEventContent" HashTable parameter, so you can use
// it to pass in arbitrary data.
handlers.RoomEventRaised = function (args) {
    var eventData = args.Data;
    log.debug("Event Raised - Game: " + args.GameId + " Event Type: " + eventData.eventType);

    switch (eventData.eventType) {
        case "playerMove":
            processPlayerMove(eventData);
            break;

        default:
            break;
    }
};
handlers.getVRRigData = function (args, context) {
    var VRRigData = {
        allcosmetics: "Early Access Supporter PackLBAAA.LBAAB.LBAAC.LBAAD.LBAAF.LBAAG.LBAAH.LBAAI.LBAAJ.LFAAA.LFAAB.LFAAC.LFAAD.LFAAE.LFAAF.LFAAG.LFAAH.LFAAI.LFAAJ.LFAAK.LFAAL.LFAAM.LFAAN.LFAAO.LHAAA.LHAAB.LHAAC.LHAAD.LHAAE.LHAAF.LHAAH.LHAAI.LHAAJ.LHAAK.LHAAL.LHAAM.LHAAN.LHAAO.LHAAP.LHAAQ.LHAAR.LHAAS.FIRST LOGINLHAAG.LBAAE.LBAAK.LHAAT.LHAAU.LHAAV.LHAAW.LHAAX.LHAAY.LHAAZ.LFAAP.LFAAQ.LFAAR.LFAAS.LFAAT.LFAAU.LBAAL.LBAAM.LBAAN.LBAAO.LSAAA.LSAAB.LSAAC.LSAAD.LHABA.LHABB.LHABC.LFAAV.LFAAW.LBAAP.LBAAQ.LBAAR.LBAAS.LFAAX.LFAAY.LFAAZ.LFABA.LHABD.LHABE.LHABF.LHABG.LSAAE.LFABB.LFABC.LHABH.LHABI.LHABJ.LHABK.LHABL.LHABM.LHABN.LHABO.LBAAT.LHABP.LHABQ.LHABR.LFABD.LBAAU.LBAAV.LBAAW.LBAAX.LBAAY.LBAAZ.LBABA.LBABB.LBABC.LBABD.LBABE.LFABE.LHABS.LHABT.LHABU.LHABV.LFABF.LFABG.LBABF.LBABG.LHABW.LBABH.LHABX.LHABY.LMAAA.LMAAB.LHABZ.LHACA.LBABJ.LBABK.LBABL.LMAAC.LMAAD.LMAAE.LBABI.LMAAF.LMAAG.LMAAH.LFABH.LHACB.LHACC.LFABI.LBABM.LBABN.LHACD.LMAAI.LMAAJ.LMAAK.LMAAL.LMAAM.LMAAN.LMAAO.LHACE.LFABJ.LFABK.LFABL.LFABM.LFABN.LFABO.LBABO.LBABP.CORN ON THE COBCRANBERRY CANFRYING PANLBACA.LBACB.LBACC.LBACD.LBACE.LBACF.LBACG.LBACH.LBADG.LBAFD.LBAFL.LBAFV.LBAGB.LBAGC.LBAGH.LBAGJ.LBAGL.LBAGS.LBAHK.LBAJC.LBARF.LBARG.LBASH.LBATD.LBATH.LBATK.LBATY.LBAUF.LBAVG.LBAVH.LBAVJ.LBAVK.LFABP.LFABQ.LFABR.LFABI.LFABH.LFABG.LFABF.LFABE.LFABO.LFABN.LFABZ.LFACA.LHADD.LHADC.LHACH.LHACG.LHACF.LHACE.LHACD.LHACC.LHACB.LHACA.LHABZ.LHABY.LHABX.LHABW.LHADG.headmodelTURKEY TOYTURKEY LEG 22PIE SLICEPIE HATOVERRIDDENLMAAU.LMAAV.HIGH TECH SLINGSHOTFINGER FLAGSTICKABLE TARGETLMAAQ."
    };

    return VRRigData; 
};              
